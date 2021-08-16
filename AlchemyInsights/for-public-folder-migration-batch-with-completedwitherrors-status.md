---
title: W przypadku partii migracji folderu publicznego ze stanem CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068174"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>W przypadku partii migracji folderu publicznego ze stanem CompletedWithErrors

Wykonaj następujące czynności, aby ukończyć partię, pomijając duże/złe elementy: 
1. Zatwierdzanie pominiętych elementów w partii migracji:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Aby zatwierdzić pominięte elementy żądań migracji, które są "zsynchronizowane", ale nie zostały ukończone, użyj następującego polecenia:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Partia migracji i żądania powinny zostać wznowione i ukończone za kilka minut.


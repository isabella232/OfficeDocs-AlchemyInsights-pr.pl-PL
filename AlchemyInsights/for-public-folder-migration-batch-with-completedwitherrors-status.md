---
title: W przypadku partii migracji folderów publicznych z stanem CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744123"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>W przypadku partii migracji folderów publicznych z stanem CompletedWithErrors

Wykonaj poniższe czynności, aby ukończyć przetwarzanie partii, pomijając duże/złe elementy: 
1. Zatwierdzanie pominiętych elementów na partii migracji:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Użyj następującego polecenia, aby zatwierdzić pominięte elementy w żądaniach migracji, które są zsynchronizowane, ale nie zostały wykonane:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Partia i żądania migracji powinny zostać wznowione i wykonane w ciągu kilku minut.


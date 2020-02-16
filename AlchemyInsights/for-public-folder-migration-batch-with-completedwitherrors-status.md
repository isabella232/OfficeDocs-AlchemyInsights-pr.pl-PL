---
title: Dla partii migracji folderów publicznych ze stanem CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043607"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Dla partii migracji folderów publicznych ze stanem CompletedWithErrors

Wykonaj następujące kroki, aby zakończyć partię, pomijając duże/złe elementy: 
1. Zatwierdzanie pominiętych towarów w partii migracji:

    Nazwa partii \<Set-MigrationBatch> -ApproveSkippedItems 
2. Użyj następującego polecenia, aby zatwierdzić pominięte elementy żądań migracji, które są "zsynchronizowane", ale nie zostały ukończone:

    $pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i w $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}
3. Partia migracji i żądania powinny zostać wznowione i zakończone w ciągu kilku minut.


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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158626"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="aa1c2-102">Dla partii migracji folderów publicznych ze stanem CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="aa1c2-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="aa1c2-103">Wykonaj następujące kroki, aby zakończyć partię, pomijając duże/złe elementy:</span><span class="sxs-lookup"><span data-stu-id="aa1c2-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="aa1c2-104">Zatwierdzanie pominiętych towarów w partii migracji:</span><span class="sxs-lookup"><span data-stu-id="aa1c2-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="aa1c2-105">Użyj następującego polecenia, aby zatwierdzić pominięte elementy żądań migracji, które są "zsynchronizowane", ale nie zostały ukończone:</span><span class="sxs-lookup"><span data-stu-id="aa1c2-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="aa1c2-106">Partia migracji i żądania powinny zostać wznowione i zakończone w ciągu kilku minut.</span><span class="sxs-lookup"><span data-stu-id="aa1c2-106">The migration batch and requests should resume and complete in a few minutes.</span></span>


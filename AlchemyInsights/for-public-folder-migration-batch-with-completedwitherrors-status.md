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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="914c8-102">Dla partii migracji folderów publicznych ze stanem CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="914c8-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="914c8-103">Wykonaj następujące kroki, aby zakończyć partię, pomijając duże/złe elementy:</span><span class="sxs-lookup"><span data-stu-id="914c8-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="914c8-104">Zatwierdzanie pominiętych towarów w partii migracji:</span><span class="sxs-lookup"><span data-stu-id="914c8-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="914c8-105">Nazwa partii \<Set-MigrationBatch> -ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="914c8-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="914c8-106">Użyj następującego polecenia, aby zatwierdzić pominięte elementy żądań migracji, które są "zsynchronizowane", ale nie zostały ukończone:</span><span class="sxs-lookup"><span data-stu-id="914c8-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="914c8-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i w $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="914c8-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="914c8-108">Partia migracji i żądania powinny zostać wznowione i zakończone w ciągu kilku minut.</span><span class="sxs-lookup"><span data-stu-id="914c8-108">The migration batch and requests should resume and complete in a few minutes.</span></span>


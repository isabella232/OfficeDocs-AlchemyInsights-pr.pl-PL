---
title: Przywracanie usuniętej witryny
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: d37fd903c91c8cd6ac6137e815cb253f7edb4494
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912685"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="b69a4-102">Przywracanie usuniętej witryny</span><span class="sxs-lookup"><span data-stu-id="b69a4-102">Restore a deleted site</span></span>

<span data-ttu-id="b69a4-103">Gdy administrator usuwa witrynę programu SharePoint, jest ona umieszczana w Koszu zbioru witryn, gdzie jest przechowywana przez 93 dni, zanim zostanie trwale usunięta.</span><span class="sxs-lookup"><span data-stu-id="b69a4-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="b69a4-104">Aby przywrócić witrynę:</span><span class="sxs-lookup"><span data-stu-id="b69a4-104">To restore the site:</span></span>
  
1. <span data-ttu-id="b69a4-105">W nowym centrum administracyjnym programu SharePoint kliknij pozycję **Kosz** na wstążce.</span><span class="sxs-lookup"><span data-stu-id="b69a4-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="b69a4-106">Zaznacz pole wyboru obok zbioru witryn, który chcesz przywrócić.</span><span class="sxs-lookup"><span data-stu-id="b69a4-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="b69a4-107">Kliknij **pozycję Przywróć elementy usunięte**.</span><span class="sxs-lookup"><span data-stu-id="b69a4-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="b69a4-108">Aby przywrócić usuniętą witrynę komunikacyjną, można użyć nowego centrum administracyjnego programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b69a4-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="b69a4-109">W przeciwnym razie należy użyć programu Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b69a4-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="b69a4-110">Aby przywrócić witrynę należącą do grupy usługi Microsoft 365, należy przywrócić grupę w centrum administracyjnym programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="b69a4-110">To restore a site that belongs to an Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="b69a4-111">Grupy można przywrócić przez 30 dni po ich usunięciu.</span><span class="sxs-lookup"><span data-stu-id="b69a4-111">Groups can be restored for 30 days after they're deleted.</span></span>
  


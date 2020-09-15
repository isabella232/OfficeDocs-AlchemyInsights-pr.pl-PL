---
title: Przywracanie usuniętej witryny
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692053"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="77da6-102">Przywracanie usuniętej witryny</span><span class="sxs-lookup"><span data-stu-id="77da6-102">Restore a deleted site</span></span>

<span data-ttu-id="77da6-103">Gdy administrator usunie witrynę programu SharePoint, jest ona umieszczana w koszu zbioru witryn, gdzie jest przechowywana przez 93 dni przed trwałym usunięciem.</span><span class="sxs-lookup"><span data-stu-id="77da6-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="77da6-104">Aby przywrócić witrynę:</span><span class="sxs-lookup"><span data-stu-id="77da6-104">To restore the site:</span></span>
  
1. <span data-ttu-id="77da6-105">W nowym centrum administracyjnym programu SharePoint kliknij pozycję **Kosz** na Wstążce.</span><span class="sxs-lookup"><span data-stu-id="77da6-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="77da6-106">Zaznacz pole wyboru obok zbioru witryn, który chcesz przywrócić.</span><span class="sxs-lookup"><span data-stu-id="77da6-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="77da6-107">Kliknij pozycję **Przywróć elementy usunięte**.</span><span class="sxs-lookup"><span data-stu-id="77da6-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="77da6-108">Aby przywrócić usuniętą witrynę komunikacyjną, możesz użyć nowego centrum administracyjnego programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="77da6-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="77da6-109">W przeciwnym razie musisz użyć programu Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="77da6-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="77da6-110">Aby przywrócić witrynę należącą do grupy programu Microsoft 365, należy przywrócić grupę w centrum administracyjnym programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="77da6-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="77da6-111">Grupy można przywracać po upływie 30 dni od ich usunięcia.</span><span class="sxs-lookup"><span data-stu-id="77da6-111">Groups can be restored for 30 days after they're deleted.</span></span>
  


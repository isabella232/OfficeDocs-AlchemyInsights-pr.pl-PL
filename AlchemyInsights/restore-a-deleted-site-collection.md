---
title: Przywracanie usuniętej witryny
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 9e4e9ade058c60ecd7a6ce1b2a40c4996ac5676f
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36552485"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="c35ed-102">Przywracanie usuniętej witryny</span><span class="sxs-lookup"><span data-stu-id="c35ed-102">Restore a deleted site</span></span>

<span data-ttu-id="c35ed-103">Gdy administrator usunie witrynę, zostanie umieszczona w koszu zbioru witryn, gdzie jest przechowywana przez 93 dni, zanim zostanie trwale usunięta.</span><span class="sxs-lookup"><span data-stu-id="c35ed-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="c35ed-104">Aby przywrócić witrynę:</span><span class="sxs-lookup"><span data-stu-id="c35ed-104">To restore the site:</span></span>
  
1. <span data-ttu-id="c35ed-105">W nowym centrum administracyjnym programu SharePoint kliknij **Kosz** na Wstążce.</span><span class="sxs-lookup"><span data-stu-id="c35ed-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="c35ed-106">Zaznacz pole wyboru obok zbioru witryn, który chcesz przywrócić.</span><span class="sxs-lookup"><span data-stu-id="c35ed-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="c35ed-107">Kliknij przycisk **Przywróć usunięte elementy**.</span><span class="sxs-lookup"><span data-stu-id="c35ed-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="c35ed-108">Aby przywrócić usuniętą witrynę komunikacyjną, można użyć nowego centrum administracyjnego programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c35ed-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="c35ed-109">W przeciwnym razie należy użyć programu Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c35ed-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="c35ed-110">Aby przywrócić witrynę należącą do grupy 365 pakietu Office, należy przywrócić grupę w centrum administracyjnym programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="c35ed-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="c35ed-111">Grupy można przywracać przez 30 dni po ich usunięciu.</span><span class="sxs-lookup"><span data-stu-id="c35ed-111">Groups can be restored for 30 days after they're deleted.</span></span>
  


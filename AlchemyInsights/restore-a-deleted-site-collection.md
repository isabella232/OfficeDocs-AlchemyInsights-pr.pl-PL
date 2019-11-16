---
title: Przywracanie usuniętej witryny
ms.author: kaarins
author: kaarins
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: a1fb15869b9f576696de4eda4c0b2101bd6cca17
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768558"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="7473c-102">Przywracanie usuniętej witryny</span><span class="sxs-lookup"><span data-stu-id="7473c-102">Restore a deleted site</span></span>

<span data-ttu-id="7473c-103">Gdy administrator usunie witrynę programu SharePoint, zostanie umieszczona w koszu zbioru witryn, gdzie jest przechowywana przez 93 dni, zanim zostanie trwale usunięta.</span><span class="sxs-lookup"><span data-stu-id="7473c-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="7473c-104">Aby przywrócić witrynę:</span><span class="sxs-lookup"><span data-stu-id="7473c-104">To restore the site:</span></span>
  
1. <span data-ttu-id="7473c-105">W nowym centrum administracyjnym programu SharePoint kliknij **Kosz** na Wstążce.</span><span class="sxs-lookup"><span data-stu-id="7473c-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="7473c-106">Zaznacz pole wyboru obok zbioru witryn, który chcesz przywrócić.</span><span class="sxs-lookup"><span data-stu-id="7473c-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="7473c-107">Kliknij przycisk **Przywróć usunięte elementy**.</span><span class="sxs-lookup"><span data-stu-id="7473c-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="7473c-108">Aby przywrócić usuniętą witrynę komunikacyjną, można użyć nowego centrum administracyjnego programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7473c-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="7473c-109">W przeciwnym razie należy użyć programu Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7473c-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="7473c-110">Aby przywrócić witrynę należącą do grupy 365 pakietu Office, należy przywrócić grupę w centrum administracyjnym programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="7473c-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="7473c-111">Grupy można przywracać przez 30 dni po ich usunięciu.</span><span class="sxs-lookup"><span data-stu-id="7473c-111">Groups can be restored for 30 days after they're deleted.</span></span>
  


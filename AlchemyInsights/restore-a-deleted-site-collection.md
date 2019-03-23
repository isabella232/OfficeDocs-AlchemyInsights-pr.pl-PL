---
title: Przywracanie usuniętego zbioru witryn
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
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753796"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="d9e7c-102">Przywracanie usuniętego zbioru witryn</span><span class="sxs-lookup"><span data-stu-id="d9e7c-102">Restore a deleted site collection</span></span>

<span data-ttu-id="d9e7c-103">Gdy administrator usunie zbiór witryn klasyczny, jest umieszczony w zbiorze witryn Kosza, gdzie jest przechowywany 93 dni, zanim zostanie trwale usunięty.</span><span class="sxs-lookup"><span data-stu-id="d9e7c-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="d9e7c-104">Aby przywrócić zbiór witryn:</span><span class="sxs-lookup"><span data-stu-id="d9e7c-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="d9e7c-105">W Centrum administracyjnego programu SharePoint klasycznych na wstążce kliknij przycisk **Kosz** .</span><span class="sxs-lookup"><span data-stu-id="d9e7c-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="d9e7c-106">Zaznacz pole wyboru obok tego zbioru witryn, które chcesz przywrócić.</span><span class="sxs-lookup"><span data-stu-id="d9e7c-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="d9e7c-107">Kliknij **Przywracanie elementów usuniętych**.</span><span class="sxs-lookup"><span data-stu-id="d9e7c-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="d9e7c-108">Aby przywrócić witrynę usuniętych komunikacji, można użyć podglądu nowe Centrum administratora programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d9e7c-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="d9e7c-109">W przeciwnym wypadku należy użyć środowiska PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d9e7c-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="d9e7c-110">Aby przywrócić witryny, która należy do grupy usługi Office 365, należy przywrócić grupy w Centrum administracyjnego programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e7c-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="d9e7c-111">Grupy można przywrócić w ciągu 30 dni od zostaną usunięte.</span><span class="sxs-lookup"><span data-stu-id="d9e7c-111">Groups can be restored for 30 days after they're deleted.</span></span>
  


---
title: Brak przepływu pracy nie można aktywować
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762111"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="57036-102">Brak przepływu pracy nie można aktywować</span><span class="sxs-lookup"><span data-stu-id="57036-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="57036-103">W zbiorze witryn programu Microsoft SharePoint nie można dodać do listy lub biblioteki globalnego przepływu pracy wielokrotnego dostępu (takiego jak "Zatwierdzanie — SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="57036-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="57036-104">Aby rozwiązać ten problem, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="57036-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="57036-105">Otwórz główną witrynę zbioru witryn w programie SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="57036-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="57036-106">W obszarze **Obiekty witryny**wybierz pozycję **Przepływy pracy**.</span><span class="sxs-lookup"><span data-stu-id="57036-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="57036-107">W sekcji **Nowe** na wstążce **Przepływy pracy** wybierz pozycję **Przepływ pracy wielokrotnego wyboru**.</span><span class="sxs-lookup"><span data-stu-id="57036-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="57036-108">W formularzu **Utwórz przepływ pracy wielokrotnego pożycietu** wprowadź nazwę \*\* *Naprawa2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="57036-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="57036-109">W przypadku **typu platformy**kliknij pozycję Przepływ pracy **programu SharePoint 2010**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="57036-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="57036-110">W sekcji **Zapisz** na wstążce **Przepływ pracy** wybierz pozycję **Publikuj**.</span><span class="sxs-lookup"><span data-stu-id="57036-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="57036-111">W sekcji **Zarządzanie** na wstążce **Przepływ pracy** wybierz pozycję **Publikuj globalnie**.</span><span class="sxs-lookup"><span data-stu-id="57036-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="57036-112">W wyświetlonym oknie dialogowym potwierdzenia wybierz przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="57036-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="57036-113">W przeglądarce sieci Web znajdź główną witrynę zbioru witryn, a następnie przejdź do **funkcji zbioru witryn**w **ustawieniach** \> witryn .</span><span class="sxs-lookup"><span data-stu-id="57036-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="57036-114">Następnie przełącz funkcję **Przepływy pracy:**</span><span class="sxs-lookup"><span data-stu-id="57036-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="57036-115">· Jeśli funkcja jest *aktywowana,* kliknij pozycję **Dezaktywuj,** a następnie kliknij przycisk **Aktywuj**.</span><span class="sxs-lookup"><span data-stu-id="57036-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="57036-116">· Jeśli funkcja jest *wyłączona,* kliknij przycisk **Aktywuj**.</span><span class="sxs-lookup"><span data-stu-id="57036-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="57036-117">Aby uzyskać więcej informacji, zapoznaj się z poniższym [artykułem](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="57036-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


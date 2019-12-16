---
title: Brak przepływu pracy nie można aktywować
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052623"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="eecf4-102">Brak przepływu pracy nie można aktywować</span><span class="sxs-lookup"><span data-stu-id="eecf4-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="eecf4-103">W zbiorze witryn programu Microsoft SharePoint nie można dodać globalnego przepływu pracy wielokrotnego użytku (na przykład "zatwierdzanie-SharePoint 2010") do listy lub biblioteki.</span><span class="sxs-lookup"><span data-stu-id="eecf4-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="eecf4-104">Aby rozwiązać ten problem, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="eecf4-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="eecf4-105">Otwórz stronę główną witryny sieci Web zbioru witryn w programie SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="eecf4-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="eecf4-106">W obszarze **obiekty lokacji**wybierz pozycję **przepływy pracy**.</span><span class="sxs-lookup"><span data-stu-id="eecf4-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="eecf4-107">W **Nowa** sekcja na Wstążce **przepływy pracy** , wybierz **przepływu pracy wielokrotnego użytku**.</span><span class="sxs-lookup"><span data-stu-id="eecf4-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="eecf4-108">W formularzu **Tworzenie przepływu pracy wielokrotnego użytku** wprowadź nazwę \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="eecf4-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="eecf4-109">Dla **typu platformy**, kliknij przycisk **przepływu pracy programu SharePoint 2010**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="eecf4-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="eecf4-110">W **Zapisz** sekcji na Wstążce **przepływu pracy** , wybierz **publikowania**.</span><span class="sxs-lookup"><span data-stu-id="eecf4-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="eecf4-111">W sekcji **Zarządzaj** na Wstążce **przepływu pracy** wybierz **publikowania globalnie**.</span><span class="sxs-lookup"><span data-stu-id="eecf4-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="eecf4-112">W wyświetlonym oknie dialogowym potwierdzenia wybierz **przycisk OK**.</span><span class="sxs-lookup"><span data-stu-id="eecf4-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="eecf4-113">W przeglądarce sieci Web zlokalizuj głównej witryny sieci Web zbioru witryn, a następnie dostęp do \> **funkcji zbioru witryn** **Ustawienia witryny** .</span><span class="sxs-lookup"><span data-stu-id="eecf4-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="eecf4-114">Następnie Przełącz funkcję **przepływy pracy** :</span><span class="sxs-lookup"><span data-stu-id="eecf4-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="eecf4-115">· Jeśli funkcja jest *aktywna* , kliknij przycisk **Dezaktywuj,** a następnie kliknij przycisk **Aktywuj**.</span><span class="sxs-lookup"><span data-stu-id="eecf4-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="eecf4-116">· Jeśli funkcja jest *dezaktywowana* , kliknij przycisk **Aktywuj**.</span><span class="sxs-lookup"><span data-stu-id="eecf4-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="eecf4-117">Aby uzyskać więcej informacji, zapoznaj się z następującym [artykułem](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="eecf4-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


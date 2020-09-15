---
title: Nie można aktywować brakującego przepływu pracy
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667096"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="3fef4-102">Nie można aktywować brakującego przepływu pracy</span><span class="sxs-lookup"><span data-stu-id="3fef4-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="3fef4-103">W zbiorze witryn programu Microsoft SharePoint nie można dodać globalnego przepływu pracy do wielokrotnego użytku (takiego jak "zatwierdzanie — SharePoint 2010") do listy lub biblioteki.</span><span class="sxs-lookup"><span data-stu-id="3fef4-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="3fef4-104">Aby rozwiązać ten problem, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="3fef4-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="3fef4-105">Otwórz główną witrynę sieci Web zbioru witryn w programie SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="3fef4-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="3fef4-106">W obszarze **obiekty witryny**wybierz pozycję **przepływy pracy**.</span><span class="sxs-lookup"><span data-stu-id="3fef4-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="3fef4-107">W **nowej** sekcji wstążki **przepływy pracy** wybierz pozycję **przepływ pracy wielokrotnego użytku**.</span><span class="sxs-lookup"><span data-stu-id="3fef4-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="3fef4-108">W formularzu **Utwórz przepływ pracy wielokrotnego użytku** wprowadź nazwę \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="3fef4-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="3fef4-109">W obszarze **Typ platformy**kliknij pozycję **przepływ pracy programu SharePoint 2010**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="3fef4-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="3fef4-110">W sekcji **Zapisywanie** wstążki **przepływu pracy** wybierz pozycję **Publikuj**.</span><span class="sxs-lookup"><span data-stu-id="3fef4-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="3fef4-111">W sekcji **Zarządzanie** na Wstążce **przepływu pracy** wybierz pozycję **Publikuj globalnie**.</span><span class="sxs-lookup"><span data-stu-id="3fef4-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="3fef4-112">W wyświetlonym oknie dialogowym potwierdzenia wybierz **przycisk OK**.</span><span class="sxs-lookup"><span data-stu-id="3fef4-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="3fef4-113">W przeglądarce internetowej Znajdź główną witrynę sieci Web zbioru witryn, a następnie uzyskaj dostęp do **Site Settings** \> **funkcji zbioru witryn**ustawienia witryny.</span><span class="sxs-lookup"><span data-stu-id="3fef4-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="3fef4-114">Następnie Przełącz funkcję **przepływy pracy** :</span><span class="sxs-lookup"><span data-stu-id="3fef4-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="3fef4-115">· Jeśli funkcja jest  *aktywowana*  , kliknij pozycję **Dezaktywuj,** a następnie kliknij pozycję **Aktywuj**.</span><span class="sxs-lookup"><span data-stu-id="3fef4-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="3fef4-116">· Jeśli funkcja jest  *wyłączona*  , kliknij pozycję **Aktywuj**.</span><span class="sxs-lookup"><span data-stu-id="3fef4-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="3fef4-117">Więcej informacji znajdziesz w poniższym [artykule](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="3fef4-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


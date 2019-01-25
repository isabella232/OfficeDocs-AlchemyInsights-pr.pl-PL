---
title: Nie można dodać przepływ pracy zatwierdzania 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483349"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="22bf5-102">Nie można dodać przepływ pracy zatwierdzania 2010</span><span class="sxs-lookup"><span data-stu-id="22bf5-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="22bf5-103">W zbiorze witryn programu Microsoft SharePoint do wielokrotnego użytku globalnego przepływu pracy (na przykład "Zatwierdzanie — SharePoint 2010") nie można dodać do listy lub biblioteki.</span><span class="sxs-lookup"><span data-stu-id="22bf5-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="22bf5-104">Aby rozwiązać ten problem, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="22bf5-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="22bf5-105">Otwórz witrynę głównego zbioru witryn programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="22bf5-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="22bf5-106">W obszarze **Obiekty lokacji**zaznacz **przepływów pracy**.</span><span class="sxs-lookup"><span data-stu-id="22bf5-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="22bf5-107">W sekcji **Nowy** wstążki **przepływów pracy** wybierz **Przepływ pracy wielokrotnego użytku**.</span><span class="sxs-lookup"><span data-stu-id="22bf5-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="22bf5-p101">W formularzu **Tworzenie przepływu pracy wielokrotnego użytku** , wprowadź nazwę \*\* *Repair2010* \*\*. Dla **Typu platformy**kliknij **Przepływu pracy programu SharePoint 2010**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="22bf5-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="22bf5-110">W sekcji **Zapisywanie** na wstążce **przepływu pracy** wybierz **Publikowanie**.</span><span class="sxs-lookup"><span data-stu-id="22bf5-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="22bf5-p102">W sekcji **Zarządzanie** na wstążce **przepływu pracy** wybierz **Publikowanie na całym świecie**. W oknie dialogowym potwierdzenia wybierz przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="22bf5-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="22bf5-p103">W przeglądarce sieci web zlokalizuj witryny głównego zbioru witryn, a następnie uzyskać dostęp do **Ustawień witryny** \> **Funkcje zbioru witryn**. Przełączanie funkcji **przepływów pracy** :</span><span class="sxs-lookup"><span data-stu-id="22bf5-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="22bf5-115">· Jeśli funkcja jest *aktywowany* , kliknij przycisk **Dezaktywuj,** a następnie kliknij przycisk **Uaktywnij**.</span><span class="sxs-lookup"><span data-stu-id="22bf5-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="22bf5-116">· Jeśli funkcja jest *zdezaktywowane* , kliknij przycisk **Uaktywnij**.</span><span class="sxs-lookup"><span data-stu-id="22bf5-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="22bf5-117">Więcej informacji można znaleźć w następującym [artykule](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="22bf5-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


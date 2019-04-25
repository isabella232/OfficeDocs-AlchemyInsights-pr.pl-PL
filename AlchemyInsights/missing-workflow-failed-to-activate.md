---
title: Brak przepływu pracy nie powiodła się Aktywacja
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418443"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="c05b9-102">Brak przepływu pracy nie powiodła się Aktywacja</span><span class="sxs-lookup"><span data-stu-id="c05b9-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="c05b9-103">W zbiorze witryn programu Microsoft SharePoint do wielokrotnego użytku globalnego przepływu pracy (na przykład "Zatwierdzanie — SharePoint 2010") nie można dodać do listy lub biblioteki.</span><span class="sxs-lookup"><span data-stu-id="c05b9-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="c05b9-104">Aby rozwiązać ten problem, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="c05b9-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="c05b9-105">Otwórz witrynę głównego zbioru witryn programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c05b9-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="c05b9-106">W obszarze **Obiekty lokacji**zaznacz **przepływów pracy**.</span><span class="sxs-lookup"><span data-stu-id="c05b9-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="c05b9-107">W sekcji **Nowy** wstążki **przepływów pracy** wybierz **Przepływ pracy wielokrotnego użytku**.</span><span class="sxs-lookup"><span data-stu-id="c05b9-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="c05b9-108">W formularzu **Tworzenie przepływu pracy wielokrotnego użytku** , wprowadź nazwę \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="c05b9-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="c05b9-109">Dla **Typu platformy**kliknij **Przepływu pracy programu SharePoint 2010**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="c05b9-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="c05b9-110">W sekcji **Zapisywanie** na wstążce **przepływu pracy** wybierz **Publikowanie**.</span><span class="sxs-lookup"><span data-stu-id="c05b9-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="c05b9-111">W sekcji **Zarządzanie** na wstążce **przepływu pracy** wybierz **Publikowanie na całym świecie**.</span><span class="sxs-lookup"><span data-stu-id="c05b9-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="c05b9-112">W oknie dialogowym potwierdzenia wybierz przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="c05b9-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="c05b9-113">W przeglądarce sieci web zlokalizuj witryny głównego zbioru witryn, a następnie uzyskać dostęp do **Ustawień witryny** \> **Funkcje zbioru witryn**.</span><span class="sxs-lookup"><span data-stu-id="c05b9-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="c05b9-114">Następnie przełącz funkcja **przepływów pracy** :</span><span class="sxs-lookup"><span data-stu-id="c05b9-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="c05b9-115">· Jeśli funkcja jest *aktywowany* , kliknij przycisk **Dezaktywuj,** a następnie kliknij przycisk **Uaktywnij**.</span><span class="sxs-lookup"><span data-stu-id="c05b9-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="c05b9-116">· Jeśli funkcja jest *zdezaktywowane* , kliknij przycisk **Uaktywnij**.</span><span class="sxs-lookup"><span data-stu-id="c05b9-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="c05b9-117">Więcej informacji można znaleźć w następującym [artykule](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c05b9-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


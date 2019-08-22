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
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543935"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="7620a-102">Brak przepływu pracy nie powiodła się Aktywacja</span><span class="sxs-lookup"><span data-stu-id="7620a-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="7620a-103">W zbiorze witryn programu Microsoft SharePoint do wielokrotnego użytku globalnego przepływu pracy (na przykład "Zatwierdzanie — SharePoint 2010") nie można dodać do listy lub biblioteki.</span><span class="sxs-lookup"><span data-stu-id="7620a-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="7620a-104">Aby rozwiązać ten problem, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="7620a-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="7620a-105">Otwórz witrynę głównego zbioru witryn programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="7620a-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="7620a-106">W obszarze **Obiekty lokacji**zaznacz **przepływów pracy**.</span><span class="sxs-lookup"><span data-stu-id="7620a-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="7620a-107">W sekcji **Nowy** wstążki **przepływów pracy** wybierz **Przepływ pracy wielokrotnego użytku**.</span><span class="sxs-lookup"><span data-stu-id="7620a-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="7620a-108">W formularzu **Tworzenie przepływu pracy wielokrotnego użytku** , wprowadź nazwę \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="7620a-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="7620a-109">Dla **Typu platformy**kliknij **Przepływu pracy programu SharePoint 2010**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="7620a-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="7620a-110">W sekcji **Zapisywanie** na wstążce **przepływu pracy** wybierz **Publikowanie**.</span><span class="sxs-lookup"><span data-stu-id="7620a-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="7620a-111">W sekcji **Zarządzanie** na wstążce **przepływu pracy** wybierz **Publikowanie na całym świecie**.</span><span class="sxs-lookup"><span data-stu-id="7620a-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="7620a-112">W oknie dialogowym potwierdzenia wybierz przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="7620a-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="7620a-113">W przeglądarce sieci web zlokalizuj witryny głównego zbioru witryn, a następnie uzyskać dostęp do **Ustawień witryny** \> **Funkcje zbioru witryn**.</span><span class="sxs-lookup"><span data-stu-id="7620a-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="7620a-114">Następnie przełącz funkcja **przepływów pracy** :</span><span class="sxs-lookup"><span data-stu-id="7620a-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="7620a-115">· Jeśli funkcja jest *aktywowany* , kliknij przycisk **Dezaktywuj,** a następnie kliknij przycisk **Uaktywnij**.</span><span class="sxs-lookup"><span data-stu-id="7620a-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="7620a-116">· Jeśli funkcja jest *zdezaktywowane* , kliknij przycisk **Uaktywnij**.</span><span class="sxs-lookup"><span data-stu-id="7620a-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="7620a-117">Więcej informacji można znaleźć w następującym [artykule](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="7620a-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


---
title: Nie można dodać przepływu pracy zatwierdzania 2010
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748694"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="86467-102">Nie można dodać przepływu pracy zatwierdzania 2010</span><span class="sxs-lookup"><span data-stu-id="86467-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="86467-103">W zbiorze witryn programu Microsoft SharePoint nie można dodać globalnego przepływu pracy wielokrotnego użytku (na przykład "zatwierdzanie-SharePoint 2010") do listy lub biblioteki.</span><span class="sxs-lookup"><span data-stu-id="86467-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="86467-104">Aby rozwiązać ten problem, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="86467-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="86467-105">Otwórz stronę główną witryny sieci Web zbioru witryn w programie SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="86467-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="86467-106">W obszarze **obiekty lokacji**wybierz pozycję **przepływy pracy**.</span><span class="sxs-lookup"><span data-stu-id="86467-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="86467-107">W **Nowa** sekcja na Wstążce **przepływy pracy** , wybierz **przepływu pracy wielokrotnego użytku**.</span><span class="sxs-lookup"><span data-stu-id="86467-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="86467-108">W formularzu **Tworzenie przepływu pracy wielokrotnego użytku** wprowadź nazwę \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="86467-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="86467-109">Dla **typu platformy**, kliknij przycisk **przepływu pracy programu SharePoint 2010**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="86467-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="86467-110">W **Zapisz** sekcji na Wstążce **przepływu pracy** , wybierz **publikowania**.</span><span class="sxs-lookup"><span data-stu-id="86467-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="86467-111">W sekcji **Zarządzaj** na Wstążce **przepływu pracy** wybierz **publikowania globalnie**.</span><span class="sxs-lookup"><span data-stu-id="86467-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="86467-112">W wyświetlonym oknie dialogowym potwierdzenia wybierz **przycisk OK**.</span><span class="sxs-lookup"><span data-stu-id="86467-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="86467-113">W przeglądarce sieci Web zlokalizuj głównej witryny sieci Web zbioru witryn, a następnie dostęp do \> **funkcji zbioru witryn** **Ustawienia witryny** .</span><span class="sxs-lookup"><span data-stu-id="86467-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="86467-114">Przełącz funkcję **przepływy pracy** :</span><span class="sxs-lookup"><span data-stu-id="86467-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="86467-115">· Jeśli funkcja jest *aktywna* , kliknij przycisk **Dezaktywuj,** a następnie kliknij przycisk **Aktywuj**.</span><span class="sxs-lookup"><span data-stu-id="86467-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="86467-116">· Jeśli funkcja jest *dezaktywowana* , kliknij przycisk **Aktywuj**.</span><span class="sxs-lookup"><span data-stu-id="86467-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="86467-117">Aby uzyskać więcej informacji, zapoznaj się z następującym [artykułem](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="86467-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  


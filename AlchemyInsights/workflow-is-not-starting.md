---
title: Przepływ pracy nie jest uruchamiany.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270790"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="b4299-102">Przepływ pracy nie jest uruchamiany.</span><span class="sxs-lookup"><span data-stu-id="b4299-102">Workflow is not starting</span></span>

- <span data-ttu-id="b4299-103">Przepływy pracy programu SharePoint 2010 i SharePoint 2013 nie jest uruchamiany.</span><span class="sxs-lookup"><span data-stu-id="b4299-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="b4299-104">Jeśli przepływ pracy nie uruchamia się, może istnieć problem tymczasowej usługi gdzie użytkownicy mogą występować sporadyczne opóźnienia z postępu przepływu pracy.</span><span class="sxs-lookup"><span data-stu-id="b4299-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="b4299-105">Sprawdź [Pulpit nawigacyjny kondycji usługi](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , by zobaczyć, jeśli dotyczy to organizacji.</span><span class="sxs-lookup"><span data-stu-id="b4299-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="b4299-106">Jeśli więcej niż 24 godziny minęło po raz pierwszy zobaczył ten problem, należy zalogować się do pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="b4299-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b4299-107">W wielu przypadkach już pracujemy nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="b4299-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b4299-108">Podaj co najmniej 24 godziny, aby ukończyć rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="b4299-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="b4299-109">Na ekranie startowym opóźnione przepływy pracy programu SharePoint 2010.</span><span class="sxs-lookup"><span data-stu-id="b4299-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="b4299-110">Dzieje się tak, jeśli przepływ pracy zostanie wywołany w dużych partii.</span><span class="sxs-lookup"><span data-stu-id="b4299-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="b4299-111">(na przykład, kiedy kilka przedmiotów są dodawane na raz).</span><span class="sxs-lookup"><span data-stu-id="b4299-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="b4299-112">Przepływy pracy nie są przeznaczone do uruchamiania w czasie rzeczywistym, więc opóźnienia jest zachowanie przez projekt.</span><span class="sxs-lookup"><span data-stu-id="b4299-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="b4299-113">Jeśli przepływ pracy zostanie złożona Extensible obiektu Markup Language (XMOL), kompilacja może być powolne.</span><span class="sxs-lookup"><span data-stu-id="b4299-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="b4299-114">Sprawdź [w tym](https://support.microsoft.com/en-us/kb/3043697) artykule.</span><span class="sxs-lookup"><span data-stu-id="b4299-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="b4299-115">Należy uprościć przepływu pracy lub wprowadzanie zmian w projekcie przy użyciu typu platformy przepływu pracy programu Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="b4299-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="b4299-116">Jeśli historii przepływu pracy wzrosła duże, warto Przeczyść elementy lub utworzyć nową listę historii.</span><span class="sxs-lookup"><span data-stu-id="b4299-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="b4299-117">Więcej informacji: [przeczyścić historię przepływu pracy](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="b4299-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="b4299-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="b4299-118">Related topics</span></span>
<span data-ttu-id="b4299-119">Czy chcesz spróbować Flow Microsoft w dokumentacji Online programu SharePoint?</span><span class="sxs-lookup"><span data-stu-id="b4299-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="b4299-120">Utworzyć przepływ</span><span class="sxs-lookup"><span data-stu-id="b4299-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="b4299-121">SharePoint i przepływu</span><span class="sxs-lookup"><span data-stu-id="b4299-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



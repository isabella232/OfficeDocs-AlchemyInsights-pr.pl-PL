---
title: Przepływ pracy nie jest rozpoczynany
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
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738099"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="5790b-102">Przepływ pracy nie jest rozpoczynany</span><span class="sxs-lookup"><span data-stu-id="5790b-102">Workflow is not starting</span></span>

- <span data-ttu-id="5790b-103">Nie są uruchamianie przepływów pracy programu SharePoint 2010 i SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="5790b-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="5790b-104">Jeśli przepływ pracy nie jest uruchamianie, może być problem tymczasowy usługi, gdzie użytkownicy mogą wystąpić sporadyczne opóźnienia z postępu przepływu pracy.</span><span class="sxs-lookup"><span data-stu-id="5790b-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="5790b-105">Sprawdź [pulpit nawigacyjny kondycji usługi](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , aby sprawdzić, czy Twoja organizacja ma wpływ.</span><span class="sxs-lookup"><span data-stu-id="5790b-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="5790b-106">Jeśli minęło więcej niż 24 godziny od pierwszego zobaczyłem ten problem, należy zalogować bilet pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="5790b-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="5790b-107">W wielu przypadkach pracujemy już nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="5790b-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="5790b-108">Proszę dać nam co najmniej 24 godziny, aby zakończyć rozwiązanie.</span><span class="sxs-lookup"><span data-stu-id="5790b-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="5790b-109">Przepływy pracy programu SharePoint 2010 opóźnione podczas uruchamiania.</span><span class="sxs-lookup"><span data-stu-id="5790b-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="5790b-110">Dzieje się tak, jeśli przepływ pracy jest wyzwalany w dużych partiach.</span><span class="sxs-lookup"><span data-stu-id="5790b-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="5790b-111">(na przykład, gdy kilka elementów są dodawane jednocześnie).</span><span class="sxs-lookup"><span data-stu-id="5790b-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="5790b-112">Przepływy pracy nie są przeznaczone do uruchamiania w czasie rzeczywistym, więc opóźnienie jest zachowanie przez projekt.</span><span class="sxs-lookup"><span data-stu-id="5790b-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="5790b-113">Jeśli przepływ pracy jest złożony Extensible Object Markup Language (XMOL), kompilacja może być powolne.</span><span class="sxs-lookup"><span data-stu-id="5790b-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="5790b-114">Sprawdź [ten](https://support.microsoft.com//kb/3043697) artykuł.</span><span class="sxs-lookup"><span data-stu-id="5790b-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="5790b-115">Należy uprościć przepływ pracy lub przeprojektować go przy użyciu typu platformy Microsoft SharePoint 2013 przepływu pracy.</span><span class="sxs-lookup"><span data-stu-id="5790b-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="5790b-116">Jeśli Historia przepływu pracy wzrosła, możesz chcieć usunąć elementy lub utworzyć nową listę historii.</span><span class="sxs-lookup"><span data-stu-id="5790b-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="5790b-117">Więcej informacji: [Wyczyść historię przepływu pracy](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="5790b-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="5790b-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="5790b-118">Related topics</span></span>
<span data-ttu-id="5790b-119">Chcesz wypróbować usługi Microsoft Flow w usłudze SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="5790b-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="5790b-120">Utwórz przepływ</span><span class="sxs-lookup"><span data-stu-id="5790b-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="5790b-121">SharePoint i przepływu</span><span class="sxs-lookup"><span data-stu-id="5790b-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



---
title: Przepływ pracy nie jest uruchamiany
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766107"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="6ff5a-102">Przepływ pracy nie jest uruchamiany</span><span class="sxs-lookup"><span data-stu-id="6ff5a-102">Workflow is not starting</span></span>

- <span data-ttu-id="6ff5a-103">Nie uruchamiają się przepływów pracy programu SharePoint 2010 i SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="6ff5a-104">Jeśli przepływ pracy nie jest uruchamiany, może to być tymczasowy problem z usługą, w którym użytkownicy mogą doświadczać sporadyczne opóźnienia z postępem przepływu pracy.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="6ff5a-105">Sprawdź pulpit nawigacyjny [kondycji usługi,](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) aby sprawdzić, czy twoja organizacja ma wpływ.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="6ff5a-106">Jeśli od pierwszego zobaczenia tego problemu minęło więcej niż 24 godziny, zarejestruj bilet pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="6ff5a-107">W wielu przypadkach już pracujemy nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="6ff5a-108">Daj nam co najmniej 24 godziny na uzupełnienie rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="6ff5a-109">Przepływy pracy programu SharePoint 2010 opóźnione przy uruchomieniu.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="6ff5a-110">Dzieje się tak, jeśli przepływ pracy jest wyzwalany w dużych partiach.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="6ff5a-111">(na przykład, gdy kilka elementów są dodawane naraz).</span><span class="sxs-lookup"><span data-stu-id="6ff5a-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="6ff5a-112">Przepływy pracy nie są przeznaczone do uruchamiania w czasie rzeczywistym, więc opóźnienie jest zachowaniem według projektu.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="6ff5a-113">Jeśli przepływ pracy jest złożony extensible Object Markup Language (XMOL), kompilacja może być powolna.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="6ff5a-114">Sprawdź [ten](https://support.microsoft.com//kb/3043697) artykuł.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="6ff5a-115">Należy uprościć przepływ pracy lub przeprojektować go przy użyciu typu platformy przepływów pracy programu Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="6ff5a-116">Jeśli historia przepływu pracy stała się duża, można przeczyścić elementy lub utworzyć nową listę historii.</span><span class="sxs-lookup"><span data-stu-id="6ff5a-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="6ff5a-117">Więcej informacji : [Historia przepływu pracy przeczyszczanie](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="6ff5a-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="6ff5a-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="6ff5a-118">Related topics</span></span>
<span data-ttu-id="6ff5a-119">Chcesz wypróbować usługę Microsoft Flow w usłudze SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="6ff5a-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="6ff5a-120">Utwórz przepływ</span><span class="sxs-lookup"><span data-stu-id="6ff5a-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6ff5a-121">Program SharePoint i przepływ</span><span class="sxs-lookup"><span data-stu-id="6ff5a-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



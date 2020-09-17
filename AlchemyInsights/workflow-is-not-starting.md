---
title: Przepływ pracy nie jest uruchamiany
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794777"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="2c658-102">Przepływ pracy nie jest uruchamiany</span><span class="sxs-lookup"><span data-stu-id="2c658-102">Workflow is not starting</span></span>

- <span data-ttu-id="2c658-103">Nie można uruchomić przepływów pracy programu SharePoint 2010 i SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="2c658-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="2c658-104">Jeśli przepływ pracy nie rozpoczyna się, może to oznaczać, że wystąpił tymczasowy problem z usługą, w którym użytkownicy mogą napotykać sporadycznie opóźnienia z postępem przepływu pracy.</span><span class="sxs-lookup"><span data-stu-id="2c658-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="2c658-105">Sprawdź [pulpit nawigacyjny kondycji usługi](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , aby sprawdzić, czy Twoja organizacja ma wpływ na.</span><span class="sxs-lookup"><span data-stu-id="2c658-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="2c658-106">Jeśli od momentu pierwszego uruchomienia tego problemu minęło więcej niż 24 godziny, zarejestruj bilet pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="2c658-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="2c658-107">W wielu przypadkach jesteśmy już nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="2c658-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2c658-108">Przekaż nam co najmniej 24 godziny na zakończenie rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="2c658-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="2c658-109">Przepływy pracy programu SharePoint 2010 opóźnione od uruchomienia.</span><span class="sxs-lookup"><span data-stu-id="2c658-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="2c658-110">Dzieje się tak, jeśli przepływ pracy zostanie wyzwolony w dużych partiach.</span><span class="sxs-lookup"><span data-stu-id="2c658-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="2c658-111">(na przykład po dodaniu kilku elementów jednocześnie).</span><span class="sxs-lookup"><span data-stu-id="2c658-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="2c658-112">Przepływy pracy nie są przeznaczone do uruchamiania w czasie rzeczywistym, więc zachowanie polega na zaprojektowaniu.</span><span class="sxs-lookup"><span data-stu-id="2c658-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="2c658-113">Jeśli przepływ pracy jest skomplikowanym językiem Extensible Object Markup Language (XMOL), kompilacja może potrwać wolno.</span><span class="sxs-lookup"><span data-stu-id="2c658-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="2c658-114">Sprawdź [ten](https://support.microsoft.com//kb/3043697) artykuł.</span><span class="sxs-lookup"><span data-stu-id="2c658-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="2c658-115">W celu uproszczenia przepływu pracy lub zaprojektowania go możesz go ponownie użyć na platformie przepływu pracy programu Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="2c658-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="2c658-116">Jeśli Historia przepływu pracy jest duża, możesz chcieć przeczyścić te elementy lub utworzyć nową listę historii.</span><span class="sxs-lookup"><span data-stu-id="2c658-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="2c658-117">Więcej informacji: [przeczyszczanie historii przepływu pracy](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="2c658-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="2c658-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="2c658-118">Related topics</span></span>
<span data-ttu-id="2c658-119">Chcesz wypróbować przepływ pracy Microsoft w usłudze SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="2c658-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="2c658-120">Utwórz przepływ</span><span class="sxs-lookup"><span data-stu-id="2c658-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2c658-121">Program SharePoint i przepływ</span><span class="sxs-lookup"><span data-stu-id="2c658-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



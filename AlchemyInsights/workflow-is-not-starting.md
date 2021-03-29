---
title: Przepływ pracy nie jest rozpoczynany
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403753"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="61dac-102">Przepływ pracy nie jest rozpoczynany</span><span class="sxs-lookup"><span data-stu-id="61dac-102">Workflow is not starting</span></span>

- <span data-ttu-id="61dac-103">Przepływy pracy programu SharePoint 2010 i SharePoint 2013 nie są rozpoczynane.</span><span class="sxs-lookup"><span data-stu-id="61dac-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="61dac-104">Jeśli przepływ pracy nie jest rozpoczynany, może wystąpić tymczasowy problem z usługą, w przypadku którego użytkownicy mogą mieć sporadyczne opóźnienia z postępem przepływu pracy.</span><span class="sxs-lookup"><span data-stu-id="61dac-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="61dac-105">Sprawdź na [pulpicie nawigacyjnym kondycji](https://admin.microsoft.com/AdminPortal/Home/servicehealth) usług, czy wpływa to na Twoją organizację.</span><span class="sxs-lookup"><span data-stu-id="61dac-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="61dac-106">Jeśli od pierwszego problemu minęły ponad 24 godziny, zaloguj bilet pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="61dac-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="61dac-107">W wielu przypadkach pracujemy już nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="61dac-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="61dac-108">Daj nam co najmniej 24 godziny, aby ukończyć rozwiązanie.</span><span class="sxs-lookup"><span data-stu-id="61dac-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="61dac-109">Przepływy pracy programu SharePoint 2010 opóźnione po uruchomieniu.</span><span class="sxs-lookup"><span data-stu-id="61dac-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="61dac-110">Dzieje się tak, jeśli przepływ pracy jest wyzwalany w dużych partiach.</span><span class="sxs-lookup"><span data-stu-id="61dac-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="61dac-111">(na przykład gdy kilka elementów jest dodawanych jednocześnie).</span><span class="sxs-lookup"><span data-stu-id="61dac-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="61dac-112">Przepływy pracy nie są zaprojektowane do uruchamiania w czasie rzeczywistym, więc opóźnienie jest procesem projektu.</span><span class="sxs-lookup"><span data-stu-id="61dac-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="61dac-113">Jeśli przepływ pracy jest złożonym językiem X JIM (Extensible Object Markup Language), kompilacja może być spowalniana.</span><span class="sxs-lookup"><span data-stu-id="61dac-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="61dac-114">Zapoznaj się [z tym](https://support.microsoft.com//kb/3043697) artykułem.</span><span class="sxs-lookup"><span data-stu-id="61dac-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="61dac-115">Należy uprościć przepływ pracy lub przeprojektować go przy użyciu typu platformy przepływów pracy programu Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="61dac-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="61dac-116">Jeśli Twoja historia przepływu pracy się powiększy, możesz usunąć elementy lub utworzyć nową listę historii.</span><span class="sxs-lookup"><span data-stu-id="61dac-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="61dac-117">Więcej informacji: [Przeczyszczanie historii przepływu pracy](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="61dac-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="61dac-118">Tematy pokrewne</span><span class="sxs-lookup"><span data-stu-id="61dac-118">Related topics</span></span>
<span data-ttu-id="61dac-119">Chcesz wypróbować usługę Microsoft Flow w usłudze SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="61dac-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="61dac-120">Tworzenie przepływu</span><span class="sxs-lookup"><span data-stu-id="61dac-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="61dac-121">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="61dac-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 

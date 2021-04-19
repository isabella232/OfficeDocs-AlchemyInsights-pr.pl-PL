---
title: Wprowadzenie do wydarzeń na żywo w aplikacji Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811970"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="31b6c-102">Wprowadzenie do wydarzeń na żywo w aplikacji Teams</span><span class="sxs-lookup"><span data-stu-id="31b6c-102">Getting started with Teams live events</span></span>

<span data-ttu-id="31b6c-103">Wydarzenia na żywo w aplikacji Microsoft Teams to rozszerzenie spotkań w aplikacji Teams umożliwiające planowanie i realizację wydarzeń transmitowanych strumieniowo dla dużej publiczności online.</span><span class="sxs-lookup"><span data-stu-id="31b6c-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="31b6c-104">Aby utworzyć wydarzenie na żywo, potrzebne są następujące elementy:</span><span class="sxs-lookup"><span data-stu-id="31b6c-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="31b6c-105">Najpierw upewnij się, że wydarzenia na żywo aplikacji Teams są dostępne w [Twoim kraju i regionie](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Wydarzenia na żywo nie są jeszcze obsługiwane w niektórych krajach.</span><span class="sxs-lookup"><span data-stu-id="31b6c-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="31b6c-106">Jeśli przypisano licencje i ustawiono zasady, ale nadal nie możesz utworzyć wydarzenia na żywo w aplikacji Teams, prawdopodobnie jesteś w kraju lub regionie, w którym wydarzenia na żywo nie są jeszcze dostępne.</span><span class="sxs-lookup"><span data-stu-id="31b6c-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="31b6c-107">Licencja usługi [Office 365 Enterprise E1, E3 lub E5 bądź Office 365 A3 lub A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="31b6c-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="31b6c-108">**Uwaga**: ze względu na obserwowany w ostatnim czasie wzrost użycia usługi Teams pełne skonfigurowanie użytkownika po przypisaniu mu licencji usługi Teams może potrwać około 24 godzin.</span><span class="sxs-lookup"><span data-stu-id="31b6c-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="31b6c-109">Do tego czasu użytkownik może nie mieć dostępu do niektórych funkcji aplikacji Teams, takich jak połączenia i konferencje głosowe, i nie będzie można przypisać mu zasad usługi Teams.</span><span class="sxs-lookup"><span data-stu-id="31b6c-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="31b6c-110">Uprawnienie do [tworzenia wydarzeń na żywo w centrum administracyjnym usługi Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="31b6c-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="31b6c-111">Uprawnienie do [tworzenia wydarzeń na żywo w usłudze Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (w przypadku wydarzeń realizowanych za pomocą zewnętrznych usług lub urządzeń do obsługi transmisji).</span><span class="sxs-lookup"><span data-stu-id="31b6c-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="31b6c-112">Pełne członkostwo w zespole wewnątrz organizacji (nie możesz być gościem ani użytkownikiem z innej organizacji).</span><span class="sxs-lookup"><span data-stu-id="31b6c-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="31b6c-113">Włączone funkcje planowania spotkań prywatnych, udostępniania ekranu oraz udostępniania wideo IP w zasadach spotkań aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="31b6c-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="31b6c-114">[Najlepsze rozwiązania](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) dotyczące wydarzeń na żywo w usłudze Teams.</span><span class="sxs-lookup"><span data-stu-id="31b6c-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="31b6c-115">Aby uzyskać więcej informacji, zobacz [Wprowadzenie do wydarzeń na żywo w aplikacji Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="31b6c-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>
---
title: Dynamics 365 — niewłaściwy pulpit nawigacyjny w interfejsie systemu Dynamics 365 ujednolicony
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711285"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="d3cb8-102">Niewłaściwy pulpit nawigacyjny w usłudze Dynamics 365 Unified Interface</span><span class="sxs-lookup"><span data-stu-id="d3cb8-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="d3cb8-103">Istnieje kilka powodów, dla których może być widoczny inny pulpit nawigacyjny niż oczekiwano:</span><span class="sxs-lookup"><span data-stu-id="d3cb8-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="d3cb8-104">Użytkownik ustawił domyślny pulpit nawigacyjny użytkownika</span><span class="sxs-lookup"><span data-stu-id="d3cb8-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="d3cb8-105">Zazwyczaj można określić domyślny pulpit nawigacyjny użytkownika, jeśli przycisk **Ustaw jako domyślny** nie jest widoczny na pasku poleceń pulpitu nawigacyjnego.</span><span class="sxs-lookup"><span data-stu-id="d3cb8-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="d3cb8-106">Domyślny pulpit nawigacyjny użytkownika zastąpi wszystkie inne domyślne pulpity nawigacyjne, nawet jeśli domyślny pulpit nawigacyjny użytkownika nie znajduje się w bieżącej aplikacji.</span><span class="sxs-lookup"><span data-stu-id="d3cb8-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="d3cb8-107">Skorzystaj z poniższej metody obejścia, aby cofnąć domyślny pulpit nawigacyjny.</span><span class="sxs-lookup"><span data-stu-id="d3cb8-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="d3cb8-108">Utwórz nowy osobisty pulpit nawigacyjny.</span><span class="sxs-lookup"><span data-stu-id="d3cb8-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="d3cb8-109">Ustaw domyślnie nowy pulpit nawigacyjny jako domyślny.</span><span class="sxs-lookup"><span data-stu-id="d3cb8-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="d3cb8-110">Usuń ten pulpit nawigacyjny.</span><span class="sxs-lookup"><span data-stu-id="d3cb8-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="d3cb8-111">Pulpit nawigacyjny jest ustawiany w obszarze mapy witryny</span><span class="sxs-lookup"><span data-stu-id="d3cb8-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="d3cb8-112">Możesz ustawić domyślny pulpit nawigacyjny organizacji, wybierając pulpit nawigacyjny i wybierając opcję "Ustaw jako domyślne" w obszarze "Dostosowywanie systemu".</span><span class="sxs-lookup"><span data-stu-id="d3cb8-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="d3cb8-113">Pulpit nawigacyjny zdefiniowany w projektancie mapy witryny będzie miał pierwszeństwo przed tym pulpitem nawigacyjnym, jeśli użytkownik ma do niego dostęp.</span><span class="sxs-lookup"><span data-stu-id="d3cb8-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="d3cb8-114">Aby użytkownicy widzieli pulpit nawigacyjny ustawiony jako domyślny dla organizacji, możesz wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="d3cb8-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="d3cb8-115">Ustaw ten pulpit nawigacyjny w obszarze mapy witryny</span><span class="sxs-lookup"><span data-stu-id="d3cb8-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="d3cb8-116">Usuwanie dostępu do pulpitu nawigacyjnego zdefiniowanego przez mapy witryny dla tych użytkowników</span><span class="sxs-lookup"><span data-stu-id="d3cb8-116">Remove access to the sitemap defined dashboard for those users</span></span>

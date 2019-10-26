---
title: Dynamics 365-niewłaściwy pulpit nawigacyjny pokazuje w Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528561"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="c0471-102">Niewłaściwa pokazuje pulpit nawigacyjny w systemie Dynamics 365 ujednoliconego interfejsu</span><span class="sxs-lookup"><span data-stu-id="c0471-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="c0471-103">Istnieje kilka powodów, dla których może zostać wyświetlony inny pulpit nawigacyjny niż ten, którego oczekujesz:</span><span class="sxs-lookup"><span data-stu-id="c0471-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="c0471-104">Użytkownik ustawił domyślny pulpit nawigacyjny użytkownika</span><span class="sxs-lookup"><span data-stu-id="c0471-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="c0471-105">Zazwyczaj można zidentyfikować domyślnego pulpitu nawigacyjnego użytkownika jest ustawiona, jeśli przycisk **Ustaw jako domyślne** nie jest wyświetlane na pasku poleceń pulpitu nawigacyjnego.</span><span class="sxs-lookup"><span data-stu-id="c0471-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="c0471-106">Domyślny pulpit nawigacyjny użytkownika zastąpi wszystkie inne domyślne pulpity nawigacyjne, nawet jeśli domyślny pulpit nawigacyjny użytkownika nie znajduje się w bieżącej aplikacji.</span><span class="sxs-lookup"><span data-stu-id="c0471-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="c0471-107">Aby cofnąć ustawienie domyślnego pulpitu nawigacyjnego, należy użyć następującego obejścia.</span><span class="sxs-lookup"><span data-stu-id="c0471-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="c0471-108">Utwórz nowy osobisty pulpit nawigacyjny.</span><span class="sxs-lookup"><span data-stu-id="c0471-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="c0471-109">Ustaw nowy pulpit nawigacyjny jako domyślny użytkownik.</span><span class="sxs-lookup"><span data-stu-id="c0471-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="c0471-110">Usuń ten pulpit nawigacyjny.</span><span class="sxs-lookup"><span data-stu-id="c0471-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="c0471-111">Pulpit nawigacyjny jest ustawiony w mapie witryny</span><span class="sxs-lookup"><span data-stu-id="c0471-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="c0471-112">Być może ustawisz domyślny pulpit nawigacyjny organizacji, wybierając pulpit nawigacyjny i wybierając opcję "Ustaw jako domyślne" w obszarze "Dostosuj system".</span><span class="sxs-lookup"><span data-stu-id="c0471-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="c0471-113">Jednak pulpit nawigacyjny zdefiniowany w projektancie mapy witryny będzie miał pierwszeństwo przed tym panelem nawigacyjnym, jeśli użytkownik ma do niego dostęp.</span><span class="sxs-lookup"><span data-stu-id="c0471-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="c0471-114">Aby użytkownicy zobaczyli pulpit nawigacyjny ustawiony jako domyślny organizacji, możesz:</span><span class="sxs-lookup"><span data-stu-id="c0471-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="c0471-115">Ustawianie tego pulpitu nawigacyjnego w mapie witryny</span><span class="sxs-lookup"><span data-stu-id="c0471-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="c0471-116">Usuwanie dostępu do pulpitu nawigacyjnego zdefiniowanego w mapie witryny dla tych użytkowników</span><span class="sxs-lookup"><span data-stu-id="c0471-116">Remove access to the sitemap defined dashboard for those users</span></span>

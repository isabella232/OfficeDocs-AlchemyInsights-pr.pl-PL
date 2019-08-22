---
title: Dynamics 365 - niewłaściwy pulpitu nawigacyjnego zawiera w jednolity interfejs Dynamics 365
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528561"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="a6e9f-102">Niewłaściwy pulpitu nawigacyjnego zawiera w jednolity interfejs Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a6e9f-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="a6e9f-103">Istnieje kilka powodów, dla których widzisz pulpitu nawigacyjnego inny niż oczekujesz:</span><span class="sxs-lookup"><span data-stu-id="a6e9f-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="a6e9f-104">Użytkownik ma ustawiony domyślny pulpit nawigacyjny użytkownika</span><span class="sxs-lookup"><span data-stu-id="a6e9f-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="a6e9f-105">Zazwyczaj można zidentyfikować użytkownika domyślnego pulpitu nawigacyjnego jest ustawiona, jeśli przycisk **Ustaw jako domyślny** nie jest wyświetlany w pasku poleceń pulpitu nawigacyjnego.</span><span class="sxs-lookup"><span data-stu-id="a6e9f-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="a6e9f-106">Domyślny pulpit nawigacyjny użytkownika zastępują wszystkie inne domyślne pulpity nawigacyjne, nawet jeśli domyślny pulpit nawigacyjny użytkownika nie znajduje się w bieżącej aplikacji.</span><span class="sxs-lookup"><span data-stu-id="a6e9f-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="a6e9f-107">Należy użyć następującego obejścia do odłączenia ich domyślnego pulpitu nawigacyjnego.</span><span class="sxs-lookup"><span data-stu-id="a6e9f-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="a6e9f-108">Utwórz nowy osobisty pulpit nawigacyjny.</span><span class="sxs-lookup"><span data-stu-id="a6e9f-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="a6e9f-109">Ustaw ten nowy pulpit nawigacyjny jako domyślnie wybranego przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="a6e9f-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="a6e9f-110">Usunięcie tego pulpitu nawigacyjnego.</span><span class="sxs-lookup"><span data-stu-id="a6e9f-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="a6e9f-111">Pulpit nawigacyjny jest ustawiona w mapie witryny</span><span class="sxs-lookup"><span data-stu-id="a6e9f-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="a6e9f-112">Może ustawiono domyślnego pulpitu nawigacyjnego organizacji zaznaczając pulpitu nawigacyjnego i wybierając opcję "Ustaw jako domyślną" w obszarze "Dostosować System".</span><span class="sxs-lookup"><span data-stu-id="a6e9f-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="a6e9f-113">Ale zdefiniowanego w Projektancie mapy witryny pulpitu nawigacyjnego mają wyższy priorytet niż ten pulpit nawigacyjny, jeśli użytkownik ma dostęp do niego.</span><span class="sxs-lookup"><span data-stu-id="a6e9f-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="a6e9f-114">Aby użytkownicy Zobacz Pulpit nawigacyjny, który został ustawiony jako domyślny organizacji, można:</span><span class="sxs-lookup"><span data-stu-id="a6e9f-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="a6e9f-115">Ustaw ten pulpit nawigacyjny mapy witryny</span><span class="sxs-lookup"><span data-stu-id="a6e9f-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="a6e9f-116">Usuwanie dostępu do pulpitu nawigacyjnego mapy witryny zdefiniowane dla tych użytkowników</span><span class="sxs-lookup"><span data-stu-id="a6e9f-116">Remove access to the sitemap defined dashboard for those users</span></span>

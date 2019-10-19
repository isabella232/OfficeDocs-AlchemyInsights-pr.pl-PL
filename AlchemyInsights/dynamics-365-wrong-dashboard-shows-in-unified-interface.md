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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528561"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Niewłaściwa pokazuje pulpit nawigacyjny w systemie Dynamics 365 ujednoliconego interfejsu

Istnieje kilka powodów, dla których może zostać wyświetlony inny pulpit nawigacyjny niż ten, którego oczekujesz:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Użytkownik ustawił domyślny pulpit nawigacyjny użytkownika 

Zazwyczaj można zidentyfikować domyślnego pulpitu nawigacyjnego użytkownika jest ustawiona, jeśli przycisk **Ustaw jako domyślne** nie jest wyświetlane na pasku poleceń pulpitu nawigacyjnego. Domyślny pulpit nawigacyjny użytkownika zastąpi wszystkie inne domyślne pulpity nawigacyjne, nawet jeśli domyślny pulpit nawigacyjny użytkownika nie znajduje się w bieżącej aplikacji.

Aby cofnąć ustawienie domyślnego pulpitu nawigacyjnego, należy użyć następującego obejścia.

1. Utwórz nowy osobisty pulpit nawigacyjny.

2. Ustaw nowy pulpit nawigacyjny jako domyślny użytkownik.

3. Usuń ten pulpit nawigacyjny.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Pulpit nawigacyjny jest ustawiony w mapie witryny

Być może ustawisz domyślny pulpit nawigacyjny organizacji, wybierając pulpit nawigacyjny i wybierając opcję "Ustaw jako domyślne" w obszarze "Dostosuj system". Jednak pulpit nawigacyjny zdefiniowany w projektancie mapy witryny będzie miał pierwszeństwo przed tym panelem nawigacyjnym, jeśli użytkownik ma do niego dostęp.

Aby użytkownicy zobaczyli pulpit nawigacyjny ustawiony jako domyślny organizacji, możesz:

* Ustawianie tego pulpitu nawigacyjnego w mapie witryny

* Usuwanie dostępu do pulpitu nawigacyjnego zdefiniowanego w mapie witryny dla tych użytkowników

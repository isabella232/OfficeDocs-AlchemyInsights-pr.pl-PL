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
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Niewłaściwy pulpitu nawigacyjnego zawiera w jednolity interfejs Dynamics 365

Istnieje kilka powodów, dla których widzisz pulpitu nawigacyjnego inny niż oczekujesz:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Użytkownik ma ustawiony domyślny pulpit nawigacyjny użytkownika 

Zazwyczaj można zidentyfikować użytkownika domyślnego pulpitu nawigacyjnego jest ustawiona, jeśli przycisk **Ustaw jako domyślny** nie jest wyświetlany w pasku poleceń pulpitu nawigacyjnego. Domyślny pulpit nawigacyjny użytkownika zastępują wszystkie inne domyślne pulpity nawigacyjne, nawet jeśli domyślny pulpit nawigacyjny użytkownika nie znajduje się w bieżącej aplikacji.

Należy użyć następującego obejścia do odłączenia ich domyślnego pulpitu nawigacyjnego.

1. Utwórz nowy osobisty pulpit nawigacyjny.

2. Ustaw ten nowy pulpit nawigacyjny jako domyślnie wybranego przez użytkownika.

3. Usunięcie tego pulpitu nawigacyjnego.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Pulpit nawigacyjny jest ustawiona w mapie witryny

Może ustawiono domyślnego pulpitu nawigacyjnego organizacji zaznaczając pulpitu nawigacyjnego i wybierając opcję "Ustaw jako domyślną" w obszarze "Dostosować System". Ale zdefiniowanego w Projektancie mapy witryny pulpitu nawigacyjnego mają wyższy priorytet niż ten pulpit nawigacyjny, jeśli użytkownik ma dostęp do niego.

Aby użytkownicy Zobacz Pulpit nawigacyjny, który został ustawiony jako domyślny organizacji, można:

* Ustaw ten pulpit nawigacyjny mapy witryny

* Usuwanie dostępu do pulpitu nawigacyjnego mapy witryny zdefiniowane dla tych użytkowników

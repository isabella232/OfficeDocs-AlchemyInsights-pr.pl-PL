---
title: Dynamics 365 — nieprawidłowy pulpit nawigacyjny pokazuje w u usługi Dynamics 365 Ujednolicony interfejs
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101492"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Nieprawidłowy pulpit nawigacyjny w ujednoliconym interfejsie usługi Dynamics 365

Istnieje kilka powodów, dla których możesz zobaczyć inny pulpit nawigacyjny niż ten, którego oczekujesz:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Użytkownik ustawił domyślny pulpit nawigacyjny użytkownika 

Domyślny pulpit nawigacyjny użytkownika można skonfigurować zwykle, jeśli przycisk Ustaw jako domyślny nie jest pokazywany na pasku poleceń pulpitu nawigacyjnego.  Domyślny pulpit nawigacyjny użytkownika zastąpi wszystkie pozostałe domyślne pulpity nawigacyjne, nawet jeśli domyślny pulpit nawigacyjny użytkownika nie znajduje się w bieżącej aplikacji.

Aby zestawić ich domyślny pulpit nawigacyjny, użyj poniższego obejścia.

1. Tworzenie nowego osobistego pulpitu nawigacyjnego.

2. Ustawianie tego nowego pulpitu nawigacyjnego jako domyślnego użytkownika.

3. Usuń ten pulpit nawigacyjny.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Pulpit nawigacyjny ustawiony na mapie witryny

Być może ustawiono domyślny pulpit nawigacyjny organizacji, wybierając pulpit nawigacyjny i wybierając pozycję "Ustaw jako domyślne" w obszarze "Dostosuj system". Jednak pulpit nawigacyjny zdefiniowany w projektancie mapy witryny będzie miał pierwszeństwo przed tym pulpitem nawigacyjnym, jeśli użytkownik ma do niego dostęp.

Aby użytkownicy widzili pulpit nawigacyjny ustawiony jako domyślny organizacji, możesz:

* Ustawianie tego pulpitu nawigacyjnego na mapie witryny

* Usuwanie dostępu tych użytkowników do zdefiniowanego pulpitu nawigacyjnego mapy witryny

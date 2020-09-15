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
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Niewłaściwy pulpit nawigacyjny w usłudze Dynamics 365 Unified Interface

Istnieje kilka powodów, dla których może być widoczny inny pulpit nawigacyjny niż oczekiwano:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Użytkownik ustawił domyślny pulpit nawigacyjny użytkownika 

Zazwyczaj można określić domyślny pulpit nawigacyjny użytkownika, jeśli przycisk **Ustaw jako domyślny** nie jest widoczny na pasku poleceń pulpitu nawigacyjnego. Domyślny pulpit nawigacyjny użytkownika zastąpi wszystkie inne domyślne pulpity nawigacyjne, nawet jeśli domyślny pulpit nawigacyjny użytkownika nie znajduje się w bieżącej aplikacji.

Skorzystaj z poniższej metody obejścia, aby cofnąć domyślny pulpit nawigacyjny.

1. Utwórz nowy osobisty pulpit nawigacyjny.

2. Ustaw domyślnie nowy pulpit nawigacyjny jako domyślny.

3. Usuń ten pulpit nawigacyjny.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Pulpit nawigacyjny jest ustawiany w obszarze mapy witryny

Możesz ustawić domyślny pulpit nawigacyjny organizacji, wybierając pulpit nawigacyjny i wybierając opcję "Ustaw jako domyślne" w obszarze "Dostosowywanie systemu". Pulpit nawigacyjny zdefiniowany w projektancie mapy witryny będzie miał pierwszeństwo przed tym pulpitem nawigacyjnym, jeśli użytkownik ma do niego dostęp.

Aby użytkownicy widzieli pulpit nawigacyjny ustawiony jako domyślny dla organizacji, możesz wykonać następujące czynności:

* Ustaw ten pulpit nawigacyjny w obszarze mapy witryny

* Usuwanie dostępu do pulpitu nawigacyjnego zdefiniowanego przez mapy witryny dla tych użytkowników

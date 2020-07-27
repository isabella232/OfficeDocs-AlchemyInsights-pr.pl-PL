---
title: Obejście blokady aktywacji na nadzorowanych urządzeniach z systemem iOS za pomocą usługi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424217"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Obejście blokady aktywacji na nadzorowanych urządzeniach z systemem iOS za pomocą usługi Intune

Możliwość ominięcia blokady aktywacji na urządzeniach z systemem iOS ułatwia odzyskiwanie po scenariuszu, w którym użytkownik włącza blokadę aktywacji na urządzeniu firmowym, a następnie opuszcza firmę.

Wymagania wstępne do pominięcia blokady aktywacji obejmują:

- Urządzenie jest "nadzorowane".
- Blokada aktywacji została pomyślnie włączona przy użyciu zasad ograniczeń urządzenia z systemem iOS w usłudze Intune.

Ponadto, omijając blokadę aktywacji, należy:

- Fizycznie posiadają urządzenie jest czyszczone.
- Skopiuj kod przed wydaniem czyszczenia.

**Uwaga:** W kodzie czyszczenia nie jest rozróżniana wielkość liter, więc znaki "-" nie są wymagane.

Aby uzyskać szczegółowe informacje, zobacz [Ominięcie blokady aktywacji na nadzorowanych urządzeniach z systemem iOS z usłudze Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**CZĘSTO ZADAWANE PYTANIA**

P: **Wydałem zdalną akcję, aby usunąć dane firmy z urządzenia, a teraz utknął w stanie oczekiwania.**

Odp.: Aby akcja zdalna została pomyślnie ukończona, urządzenie docelowe musi być w trybie online i w dobrej kondycji. W następujących sytuacjach akcja zdalna pozostaje w stanie oczekiwania przez 30 dni lub do momentu, gdy urządzenie potwierdzi polecenie, gdy urządzenie:

- Nie ma łączności.
- Traci stan zarządzania w usłudze Intune.

Jeśli uważasz, że urządzenie już nie zaewidencjonuje się i nie usunie danych firmowych, wybierz pozycję Usuń. Usunięcie powoduje usunięcie rekordu urządzenia, tak aby nie był już wyświetlany na liście urządzeń usługi Intune. Aby urządzenie ponownie stało się aktywne, jego użytkownik musi ponownie zarejestrować urządzenie.

**Pyt.: Dlaczego niektóre akcje zdalne nie są dostępne do użycia?**

Odp.: Nie wszystkie platformy obsługują wszystkie akcje urządzenia zdalnego. Następujące akcje zdalne są specyficzne dla platformy.

- Blokada aktywacji obejścia (tylko system iOS)
- Nowy start (tylko windows)
- Tryb utracony (tylko iOS)
- Lokalizowanie urządzenia (tylko w systemem iOS)
- Ponowne uruchomienie (tylko system Windows)

Aby uzyskać więcej informacji na temat każdej akcji, zobacz [Dostępne akcje urządzenia](https://docs.microsoft.com/intune/device-management#available-device-actions).
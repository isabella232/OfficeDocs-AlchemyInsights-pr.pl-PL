---
title: Lokalizowanie utraconych urządzeń z systemem iOS za pomocą usługi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440424"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Lokalizowanie utraconych urządzeń z systemem iOS za pomocą usługi Intune

Włączenie trybu utraconego na urządzeniu z systemem iOS umożliwia administratorowi wyświetlanie na ekranie blokady wiadomości i numeru telefonu kontaktowego.

Po włączeniu trybu utraconego administrator może użyć akcji Znajdź urządzenie, aby zidentyfikować fizyczną lokalizację urządzenia.

Akcja Znajdź urządzenie w usłudze Intune współpracuje z urządzeniami z systemem iOS, aby wyświetlić lokalizację określonego urządzenia na mapie.

Użycie tej akcji wymaga, aby urządzenie z systemem iOS było w:

- Tryb nadzorowany
- Tryb utracony

Aby uzyskać więcej informacji, zobacz [Włączanie trybu utraconego na urządzeniach z systemem iOS/iPadOS z usłudze Intune](https://docs.microsoft.com/intune/device-lost-mode) i [lokalizowanie utraconych lub skradzionych urządzeń z systemem iOS/iPadOS za pomocą usługi Intune](https://docs.microsoft.com/intune/device-locate).

**CZĘSTO ZADAWANE PYTANIA**

P: Wydałem zdalną akcję, aby usunąć dane firmy z urządzenia, a teraz utknął w stanie oczekiwania.

Odp.: Aby akcja zdalna została pomyślnie ukończona, urządzenie docelowe musi być w trybie online i w dobrej kondycji. W następujących sytuacjach akcja zdalna pozostaje w stanie oczekiwania przez 30 dni lub do momentu, gdy urządzenie potwierdzi polecenie:

- Gdy urządzenie nie ma łączności
- Gdy urządzenie utraci stan zarządzania w usłudze Intune

Jeśli uważasz, że urządzenie już nie zaewidencjonuje się i nie będzie można usunąć danych firmowych, wybierz pozycję Usuń. Usunięcie powoduje usunięcie rekordu urządzenia, tak aby nie był już wyświetlany na liście urządzeń usługi Intune. Jeśli urządzenie stanie się ponownie aktywne, jego użytkownik będzie musiał go ponownie zarejestrować.

Pyt.: Dlaczego niektóre akcje zdalne nie są dostępne do użycia?

Odp.: Nie wszystkie platformy obsługują wszystkie akcje urządzenia zdalnego. Następujące akcje zdalne są specyficzne dla platformy, więc są one dostępne tylko dla zaznaczonych platform.

- Blokada aktywacji obejścia (tylko system iOS)
- Nowy start (tylko windows)
- Tryb utracony (tylko iOS)
- Lokalizowanie urządzenia (tylko w systemem iOS)
- Ponowne uruchomienie (tylko system Windows)

Aby uzyskać więcej informacji na temat każdej akcji, zobacz [Dostępne akcje urządzenia](https://docs.microsoft.com/intune/device-management#available-device-actions).
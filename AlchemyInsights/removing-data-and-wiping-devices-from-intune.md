---
title: Usuwanie danych i wycieranie urządzeń z usługi Intune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440471"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Usuwanie danych i wycieranie urządzeń z usługi Intune

Akcje zdalne Dotyczące wycofywania urządzeń i czyszczenia urządzenia mogą służyć do usuwania danych firmowych zarządzanych przez usługę Intune lub do przywracania ustawień fabrycznych i przywracania ustawień domyślnych urządzenia.

1. Zaloguj się do zarządzania urządzeniami w usłudze Microsoft 365 i przejdź do **urządzenia**  >  **Wszystkie urządzenia**.
2. Wybierz urządzenie, które chcesz wyczyścić.
3. Wybierz typ zdalnego czyszczenia, które chcesz wykonać. Wycofanie powoduje usunięcie tylko informacji organizacji, a pełne czyszczenie przywraca urządzenie do ustawień fabrycznych.
4. Wybierz **pozycję Tak,** aby potwierdzić. Dopóki czyszczenie nie zostanie wykończęce, stan akcji Urządzenie jest wyświetlany jako Oczekujące na wycofanie.</br>
    Po zakończeniu akcji urządzenie przenośne nie będzie już widoczne na liście zarządzanych urządzeń.

**Uwaga** Nie można usunąć danych firmy z urządzeń przyłączonych do usługi Azure AD.

Aby uzyskać szczegółowe informacje na temat efektu akcji Wycofywanie i czyszczenie, w tym tego, co jest zachowywane i co jest usuwane, zobacz [Usuwanie urządzeń za pomocą czyszczenia, wycofywania lub ręcznego wyrejestrowywania urządzenia](https://docs.microsoft.com/intune/devices-wipe).

Aby wymazać wszystkie dane z urządzenia z systemem macOS, zobacz [Wymazywanie wszystkich danych z urządzenia z systemem macOS](https://docs.microsoft.com/intune/device-erase).
---
title: Automatyczne oczyszczanie starych urządzeń w usłudze Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555226"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatyczne oczyszczanie starych urządzeń w usłudze Intune

Usługa Intune umożliwia administratorowi skonfigurowanie przedziału czasu między 90 a 270 dniami, po czym przestarzałe urządzenia są usuwane z usługi. To ustawienie jest w całej organizacji i po aktywacji wchodzi w życie natychmiast. Wszystkie urządzenia niezaewidencjonowane na serwerze usługi Intune przez okres przekraczający to ustawienie są trwale usuwane.

**Uwaga** Tylko obiekty urządzenia MDM kwalifikują się do tej akcji oczyszczania. Obiekty urządzenia EAS są wykluczone.

Aby uzyskać dodatkowe informacje o tym, kiedy urządzenie kwalifikuje się do usunięcia na podstawie ustawienia oczyszczania urządzenia i jego "stanu":

Ustawienie: **Usuwanie urządzeń po ostatniej dacie ewidencjonowania: Tak (określona wartość (N) w określonych dniach)**

- Na podstawie wartości (N) skonfigurowanych w ustawieniu usługa Intune usuwa urządzenie w określonych dniach po jego ostatnim pomyślnym zaewidencjonowania.

Ustawienie: **Usuwanie urządzeń po ostatniej dacie zameldowania: Nie**

- 180 dni po wygaśnięciu certyfikatu urządzenia i nie odnowieniu urządzenie zostanie usunięte.

**Uwaga** W obu przypadkach urządzenie musi zostać pomyślnie zarejestrowane w usłudze Intune. Rejestracja odbywa się podczas pierwszego zaewidencjonowania urządzenia za pomocą usługi Intune.

Jeśli urządzenie pomyślnie zarejestruje się w usłudze Intune, ale nie zostanie zarejestrowane w usłudze Intune, urządzenie zostanie usunięte 270 dni po rejestracji. (90 dni, aby oznaczyć urządzenie jako odwołane, a następnie kolejne 180 dni na usunięcie rekordu).

Obecnie w konsoli usługi Intune nie istnieje mechanizm służący do określania daty wygaśnięcia certyfikacji urządzenia dla danego urządzenia.
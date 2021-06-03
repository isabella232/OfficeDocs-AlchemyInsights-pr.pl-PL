---
title: Tworzenie tagów lub grup urządzeń i zarządzanie nimi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731671"
---
# <a name="create-and-manage-device-tags-or-groups"></a>Tworzenie tagów lub grup urządzeń i zarządzanie nimi

Dodawanie tagów na urządzeniach w celu utworzenia logicznego przynależności do grupy. Tagi urządzeń obsługują prawidłowe mapowanie sieci, umożliwiając dołączanie różnych tagów w celu przechwytywania kontekstu i umożliwienia dynamicznego tworzenia list w ramach zdarzenia. Tagi mogą być używane jako filtr w widoku listy Urządzenia lub do grupowania urządzeń. Aby uzyskać więcej informacji na temat grupowania urządzeń, zobacz [Tworzenie tagów urządzeń i zarządzanie nimi.](/microsoft-365/security/defender-endpoint/machine-tags)

Do urządzeń można dodawać tagi, takie jak:

- Korzystanie z portalu

- Ustawianie wartości klucza rejestru
 
**Uwaga:** Może brakować opóźnienia między dodaniem tagu do urządzenia a jego dostępnością na liście urządzeń i na stronie urządzenia.

Aby dodać tagi urządzeń przy użyciu interfejsu API, zobacz [Dodawanie lub usuwanie interfejsu API tagów urządzeń.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)

## <a name="add-and-manage-device-tags-using-the-portal"></a>Dodawanie tagów urządzeń i zarządzanie nimi za pomocą portalu

1. Wybierz urządzenie, na którym chcesz zarządzać tagami. Możesz wybrać lub wyszukać urządzenie w dowolnym z następujących widoków:

    - **Pulpit nawigacyjny operacji zabezpieczeń** Wybierz nazwę urządzenia w sekcji Najważniejsze urządzenia z aktywnymi alertami.
    - **Kolejka alertów** — wybierz nazwę urządzenia obok ikony urządzenia w kolejce alertów.
    - **Lista Urządzenia** — wybierz nazwę urządzenia z listy urządzeń.
    - **Pole wyszukiwania** — wybierz pozycję Urządzenie z menu rozwijanego i wprowadź nazwę urządzenia.

    Możesz również przejść do strony alertu za pośrednictwem widoków pliku i adresów IP.

1. Wybierz **pozycję Zarządzaj tagami** w wierszu akcji odpowiedzi.

1. Wpisz, aby znaleźć lub utworzyć tagi.

Tagi są dodawane do widoku urządzenia i są odzwierciedlane w widoku listy Urządzenia. Następnie możesz użyć filtru Tagi, aby wyświetlić odpowiednią listę urządzeń.

Aby uzyskać więcej informacji, [zobacz Tworzenie tagów urządzeń i zarządzanie nimi.](/microsoft-365/security/defender-endpoint/machine-tags)
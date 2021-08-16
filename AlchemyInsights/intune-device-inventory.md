---
title: Intune Device Inventory
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014082"
---
# <a name="intune-device-inventory"></a>Intune Device Inventory

Blade Devices zapewnia administratorowi wgląd w informacje dla administratorów dotyczące urządzeń w ramach zarządzania w usłudze Intune na podstawie per device. Przedstawione informacje obejmują: Sprzęt, Odkryte aplikacje, Stan zgodności urządzenia i Stan konfiguracji urządzenia.

Dane dotyczące zapasów sprzętu i wykrytych aplikacji są zbierane w cyklu siedmiodniowym. Zgłoszone aplikacje i konkretne elementy sprzętu różnią się w zależności od systemu operacyjnego urządzenia i tego, czy urządzenie należy do użytkownika, czy do firmy.

Aby uzyskać więcej informacji, [zobacz Wyświetlanie szczegółów urządzenia w usłudze Intune.](https://docs.microsoft.com/intune/device-inventory)

**CZĘSTO ZADAWANE PYTANIA**

P. Nie otrzymuję pełnej listy aplikacji w spisie aplikacji obecnych w usłudze Intune zarejestrowanej Windows urządzeniach. Dlaczego nie?

O. Obecnie na komputerach z systemem są wymienione tylko nowoczesne aplikacje Windows 10, które są identyfikowane jako urządzenia firmowe. Usługa Intune nie zbiera informacji o aplikacjach Win32 zainstalowanych na tych urządzeniach.

P. Dlaczego numery telefonów nie są zbierane ze wszystkich urządzeń?

O. Telefony kategoryzowane jako urządzenia firmowe w usłudze Intune nie są oznaczone ich pełnymi numerami telefonów, na przykład w przypadku uruchamiania raportu o spisie urządzeń przenośnych. Numery telefonów własnych urządzeń są zawsze częściowo maskowane gwiazdkami (****) i są wyświetlane tylko cztery ostatnie cyfry.
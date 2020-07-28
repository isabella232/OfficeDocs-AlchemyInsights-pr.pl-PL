---
title: Spis urządzeń usługi Intune
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440472"
---
# <a name="intune-device-inventory"></a>Spis urządzeń usługi Intune

Blok Urządzenia zapewnia administratorowi wgląd w urządzenia pod zarządzaniem w usłudze Intune na podstawie na urządzenie. Wyświetlane informacje obejmują: sprzęt, odnalezione aplikacje, stan zgodności urządzeń i stan konfiguracji urządzenia.

Dane spisowe sprzętu i odnalezionych aplikacji są zbierane w cyklu siedmiodniowym. Aplikacje i określone elementy zgłaszanego sprzętu różnią się w zależności od systemu operacyjnego urządzenia i tego, czy urządzenie jest własnością osobistą, czy firmową.

Aby uzyskać więcej informacji, zobacz [Informacje o urządzeniu w usłudze Intune](https://docs.microsoft.com/intune/device-inventory).

**CZĘSTO ZADAWANE PYTANIA**

P: Nie otrzymuję pełnej listy zapasów aplikacji znajdujących się na urządzeniach z systemem Windows zarejestrowanych w usłudze Intune. Dlaczego nie?

Odp.: Obecnie tylko nowoczesne aplikacje są wyświetlane dla komputerów z systemem Windows 10, które są identyfikowane jako urządzenia firmowe. Usługa Intune nie zbiera informacji o aplikacjach Win32 zainstalowanych na tych urządzeniach.

P: Dlaczego numery telefonów nie są zbierane ze wszystkich urządzeń?

Odp.: Telefony sklasyfikowane jako urządzenia firmowe w usłudze Intune nie są identyfikowane z ich pełnym numerem telefonu, gdy na przykład uruchomisz raport o spisie urządzeń przenośnych. Numery telefonów bring-you-own-device są zawsze częściowo zamaskowane gwiazdkami (****) i pokazują tylko cztery ostatnie cyfry.
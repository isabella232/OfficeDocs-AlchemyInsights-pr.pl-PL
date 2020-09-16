---
title: Spis urządzeń w usłudze Intune
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
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667888"
---
# <a name="intune-device-inventory"></a>Spis urządzeń w usłudze Intune

Blok urządzenia zapewnia administratorowi wgląd w urządzenia w obszarze Zarządzanie w usłudze Intune na zasadzie na urządzenie. Wyświetlane informacje obejmują: Sprzęt, odnalezione aplikacje, stan zgodności urządzenia i stan konfiguracji urządzenia.

Dane spisu dla sprzętu i wykrytych aplikacji są zbierane w cyklu siedmiu dni. Aplikacje i określone elementy sprzętu są różne w zależności od systemu operacyjnego urządzenia oraz tego, czy jest to urządzenie osobiste, czy firmowe.

Aby uzyskać więcej informacji, zobacz [Wyświetlanie szczegółów urządzenia w usłudze Intune](https://docs.microsoft.com/intune/device-inventory).

**CZĘSTO ZADAWANE PYTANIA**

P: nie otrzymuję pełnej listy spisu aplikacji obecnej na urządzeniu z systemem Windows, na których zarejestrowano usługę Intune. Dlaczego nie?

O: w tym momencie są wyświetlane tylko aplikacje nowoczesne dla komputerów z systemem Windows 10, które są zidentyfikowane jako urządzenia firmowe. Usługa Intune nie gromadzi informacji o aplikacjach Win32 zainstalowanych na tych urządzeniach.

P: Dlaczego numery telefonów nie są zbierane ze wszystkich urządzeń?

A: telefony skategoryzowane jako urządzenia firmowe w usłudze Intune nie są zidentyfikowane wraz z pełnym numerem telefonu, na przykład na potrzeby uruchamiania raportu spisu urządzeń przenośnych. Poręczne numery telefonów urządzeń są zawsze częściowo maskowane znakami gwiazdki (* * * *) i są wyświetlane tylko cztery ostatnie cyfry.
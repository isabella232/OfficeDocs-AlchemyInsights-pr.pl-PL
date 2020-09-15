---
title: Klasyczne raporty dziennika inspekcji programu SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662218"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Dzienniki inspekcji programu SharePoint i usługi OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Klasyczne dzienniki inspekcji programu SharePoint

USŁUGI spo starszej inspekcji uległa migracji do dziennika ujednoliconej inspekcji (UAL). Wszystkie usługi spo starsze raporty inspekcji będą teraz obsługiwane przez UAL, a starsze sygnały inspekcji zostaną zmigrowane do UAL.

Kluczowe zmiany:

* Przycinanie nie jest dostępne w ramach funkcji.
* Wybieranie określonych zdarzeń do inspekcji jest niedostępne. Zapoznaj się z [tym dokumentem](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) , aby uzyskać pełną listę dostępnych zdarzeń, które można poddać inspekcji domyślnie.
* Opcja **Lokalizacja** w obszarze **niestandardowe raporty** jest niedostępna.
* Opcja **otwierania lub pobierania dokumentów** jest niedostępna.

[Konfigurowanie ustawień inspekcji dla zbioru witryn](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Nowoczesne dzienniki ujednoliconej inspekcji programu SharePoint i usługi OneDrive z poziomu zgodności

* [Włączanie/wyłączanie ujednoliconych rejestracji inspekcji](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

W programie SharePoint lub usłudze OneDrive nie jest wymagana żadna dodatkowa konfiguracja.

Użyj funkcji wyszukiwania rejestrowania inspekcji, aby sprawdzić aktywność plików, folderów, użytkowników, uprawnień:

* [Działania dotyczące plików i stron](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Działania dotyczące folderów](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Działania dotyczące udostępniania i żądania dostępu](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Działania synchronizacji](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Działania administracyjne witryny](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Aby uzyskać więcej informacji o tym, jak pobrać te zdarzenia, zobacz [przeszukiwanie dziennika inspekcji](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

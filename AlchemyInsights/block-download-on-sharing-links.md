---
title: Blokuj pobieranie na łączach udostępniania
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358036"
---
# <a name="block-download-on-sharing-links"></a>Blokuj pobieranie na łączach udostępniania

**Opcja Blokuj pobieranie** jest dostępna dla łączy tylko do **wyświetlania** dokumentów pakietu Office. Po wybraniu tej opcji osoby uzyskujące dostęp do pliku za pośrednictwem utworzonego łącza nie będą widzieć opcji pobierania, drukowania ani kopiowania pliku.

Administratorzy mogą kontrolować, czy ustawienie "pobieranie blokowe" jest wyświetlane tylko dla plików pakietu Office, czy nie, zmieniając `BlockDownloadLinksFileType` to ustawienie w poleceniach cmdlet [programu PowerShell set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) lub [Set-SPOSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)

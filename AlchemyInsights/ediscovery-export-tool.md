---
title: Narzędzie eksportu eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/3/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 5a54344d43d16c77d440768aa1c87489edf10ca0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36736335"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nie można zainstalować lub uruchomić narzędzia eksportu eDiscovery?

Jeśli nie można zainstalować lub uruchomić Office 365 eDiscovery Export narzędzie do pobierania wyników wyszukiwania, sprawdź następujące rzeczy:
  
- Komputer, którego używasz, spełnia te wymagania:

  - 32-lub 64-bitowe wersje systemu Windows 7 i nowsze wersje

  - Microsoft.NET Framework 4,7

  - Obsługiwana przeglądarka:

  - Program Microsoft Edge

    Lub

  - Internet Explorer 10 i nowsze wersje

    Inne przeglądarki, takie jak Google Chrome i Mozilla Firefox, nie są obsługiwane.

- Twoja organizacja może połączyć się z punktem końcowym na platformie Azure, czyli ** \*. blob.Core.Windows.NET** (symbol wieloznaczny reprezentuje unikatowy identyfikator zadania eksportu).

- Rola Eksport jest przypisywana do centrum zgodności zabezpieczeń &amp; pakietu Office 365. Domyślnie ta rola jest przypisany tylko do grupy ról eDiscovery Manager. Zobacz [przypisywanie uprawnień do zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Aby uzyskać więcej informacji, zobacz [Eksportowanie wyników wyszukiwania zawartości](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  
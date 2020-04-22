---
title: Narzędzie do eksportowania zbierania elektronicznych materiałów dowodowych
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 83f18d06006989e03ee6095e430aaf3eb5c72c09
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714780"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nie można zainstalować lub uruchomić narzędzia eksportu zbierania elektronicznych materiałów dowodowych?

Jeśli nie możesz zainstalować lub uruchomić narzędzia eksportu zbierania elektronicznych materiałów dowodowych w celu pobrania wyników wyszukiwania, sprawdź następujące elementy:
  
- Komputer, którego używasz, spełnia następujące wymagania wstępne:

  - 32- lub 64-bitowe wersje systemu Windows 7 i nowszych

  - Microsoft .NET Framework 4.7

  - Obsługiwana przeglądarka:

  - Microsoft Edge

    Lub

  - Internet Explorer 10 i nowsze wersje

    Inne przeglądarki, takie jak Google Chrome i Mozilla Firefox, nie są obsługiwane.

- Twoja organizacja może połączyć się z punktem końcowym na platformie Azure, który jest ** \*.blob.core.windows.net** (symbol wieloznaczny reprezentuje unikatowy identyfikator zadania eksportu).

- Przypisano rolę Eksportuj w Centrum zgodności zabezpieczeń &amp; usługi Microsoft 365. Domyślnie ta rola jest przypisywana tylko do grupy ról Menedżera zbierania elektronicznych materiałów dowodowych. Zobacz [Przypisywanie uprawnień zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Aby uzyskać więcej informacji, zobacz [Eksportowanie wyników wyszukiwania zawartości](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  
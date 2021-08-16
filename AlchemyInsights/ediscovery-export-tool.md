---
title: Narzędzie do eksportowania zbierania elektronicznych materiałów dowodowych
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101312"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nie możesz zainstalować lub uruchomić narzędzia eDiscovery Export Tool?

Jeśli nie możesz zainstalować lub uruchomić narzędzia eDiscovery Export Tool w celu pobrania wyników wyszukiwania, sprawdź następujące kwestie:
  
- Komputer, z których korzystasz, spełnia następujące wymagania wstępne:

  - Wersje 32- lub 64-bitowe Windows 7 i nowsze

  - Microsoft .NET Framework 4.7

  - Obsługiwana przeglądarka:

  - Microsoft Edge

    Lub

  - Internet Explorer 10 i nowsze wersje

    Inne przeglądarki, takie jak Google Chrome i Mozilla Firefox, nie są obsługiwane.

- Twoja organizacja może połączyć się z punktem końcowym na platformie Azure, czyli **\* .blob.core.windows.net** (symbol wieloznaczny reprezentuje symbol identyfikator unikatowy twojego zadania eksportu).

- Masz przypisaną rolę eksportowania w Centrum zgodności Microsoft 365 &amp; zabezpieczeń. Domyślnie ta rola jest przypisana tylko do grupy ról Menedżer zbierania elektronicznych materiałów dowodowych. Zobacz [Przypisywanie uprawnień zbierania elektronicznych materiałów dowodowych.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Aby uzyskać więcej informacji, zobacz [Eksportowanie wyników wyszukiwania zawartości.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

W przypadku eksportowania więcej niż 100 000 skrzynek pocztowych w celu pobrania wyników eksportowania należy użyć następującego programu PowerShell: Eksportowanie wyników z ponad  [100 000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)skrzynek pocztowych.
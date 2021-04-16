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
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814598"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nie możesz zainstalować lub uruchomić narzędzia eDiscovery Export Tool?

Jeśli nie możesz zainstalować lub uruchomić narzędzia eDiscovery Export Tool w celu pobrania wyników wyszukiwania, sprawdź następujące kwestie:
  
- Komputer, z których korzystasz, spełnia następujące wymagania wstępne:

  - 32- lub 64-bitowa wersja systemu Windows 7 i nowsze wersje

  - Microsoft .NET Framework 4.7

  - Obsługiwana przeglądarka:

  - Microsoft Edge

    Lub

  - Internet Explorer 10 i nowsze wersje

    Inne przeglądarki, takie jak Google Chrome i Mozilla Firefox, nie są obsługiwane.

- Twoja organizacja może połączyć się z punktem końcowym na platformie Azure, czyli **\* .blob.core.windows.net** (symbol wieloznaczny reprezentuje symbol identyfikator unikatowy twojego zadania eksportu).

- Masz przypisaną rolę eksportowania w Centrum zgodności zabezpieczeń platformy Microsoft 365. &amp; Domyślnie ta rola jest przypisana tylko do grupy ról Menedżer zbierania elektronicznych materiałów dowodowych. Zobacz [Przypisywanie uprawnień zbierania elektronicznych materiałów dowodowych.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Aby uzyskać więcej informacji, zobacz [Eksportowanie wyników wyszukiwania zawartości.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

W przypadku eksportowania więcej niż 100 000 skrzynek pocztowych w celu pobrania wyników eksportowania należy użyć następującego programu PowerShell: Eksportowanie wyników z ponad  [100 000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)skrzynek pocztowych.
---
title: 1490 — Rozwiązywanie problemów-zbieranie elektronicznych materiałów dowodowych — błędy
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277830"
---
# <a name="troubleshoot-content-search-errors"></a>Rozwiązywanie problemów z błędami wyszukiwania zawartości

Czy występują problemy z wyszukiwaniem zawartości lub uzyskiwaniem błędów podczas eksportowania wyników wyszukiwania?

Na przykład podczas uruchamiania wyszukiwania są wyświetlane następujące pytania?

- Błędy CS008 lub CS012

- Błędy serwera/przekroczenia limitu czasu

- Wystąpił błąd aplikacji

Jeśli chcesz wyszukiwać lub eksportować wyniki z dużej liczby skrzynek pocztowych (ponad 100 000 skrzynek pocztowych), otrzymujesz błędy eksportu?

W przypadku tych typów błędów ponów wyszukiwanie w poszukiwaniu nieuszkodzonych lokalizacji zawartości. Aby uzyskać więcej informacji, zobacz  [ten artykuł](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Jeśli eksportujesz więcej niż 100K skrzynek pocztowych, musisz użyć następującego programu PowerShell, aby pobrać wyniki eksportu:  [Eksportowanie wyników z ponad 100K skrzynek pocztowych](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).

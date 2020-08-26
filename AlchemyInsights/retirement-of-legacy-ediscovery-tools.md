---
title: Wycofanie starszych wersji narzędzi zbierania elektronicznych materiałów dowodowych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902630"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Wycofanie starszych wersji narzędzi zbierania elektronicznych materiałów dowodowych

W rezultacie nowych i ulepszonych funkcji zbierania elektronicznych materiałów dowodowych w centrum zgodności z programem Microsoft 365 następujące starsze narzędzia zbierania elektronicznych materiałów dowodowych i commandlets zostaną wycofane w nadchodzących miesiącach:

- [Miejscowe zbieranie elektronicznych materiałów dowodowych](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i [archiwa miejscowe](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) w centrum administracyjnym programu Exchange.

- Polecenia cmdlet programu Exchange Online PowerShell, które obsługują miejscowe archiwa zbierania elektronicznych materiałów dowodowych i miejscowe. Te polecenia cmdlet są zbiorczo identyfikowane jako polecenia cmdlet *-MailboxSearch. Obejmuje następujące polecenia cmdlet:

    - [Nowe — MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start — MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Zatrzymaj — MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Polecenie cmdlet [Search — Skrzynka pocztowa](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) w programie Exchange Online PowerShell.
- Poniższe operacje w interfejsie API usług sieci Web programu Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Zaawansowane zbieranie elektronicznych materiałów dowodowych v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Oś czasu dla emerytury**:
- **1 lipca 2020** r. Nie możesz już tworzyć nowych wyszukiwań i blokad, ale możesz uruchamiać, edytować i usuwać istniejące wyszukiwania na własne ryzyko. Pomoc techniczna firmy Microsoft nie obsługuje już zamiejscowych & zbierania elektronicznych materiałów dowodowych w pakiecie administracyjnym.
    
- **1 października 2020** r. Miejscowe zbieranie elektronicznych materiałów dowodowych & funkcje zostaną umieszczone w trybie tylko do odczytu, więc możesz usunąć tylko istniejące wyszukiwania i blokady.

**Aby uzyskać więcej informacji, zobacz**:

 - [Migrowanie starszych wyszukiwań i archiwów zbierania elektronicznych materiałów dowodowych do centrum zgodności z programem Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Wycofanie starszych wersji narzędzi zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Często zadawane pytania dotyczące archiwów zbierania elektronicznych materiałów dowodowych i miejscowych](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




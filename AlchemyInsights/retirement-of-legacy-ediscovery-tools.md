---
title: Wycofanie starszych narzędzi zbierania elektronicznych materiałów dowodowych
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798559"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Wycofanie starszych narzędzi zbierania elektronicznych materiałów dowodowych

W wyniku nowych i ulepszonych funkcji zbierania elektronicznych materiałów dowodowych w Centrum zgodności platformy Microsoft 365 następujące starsze narzędzia i polecenia zbierania elektronicznych materiałów dowodowych zostaną wycofane w nadchodzących miesiącach:

- [Zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) w miejscu i [zbierania](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) elektronicznych materiałów dowodowych w centrum administracyjnym programu Exchange.

- Polecenia cmdlet programu PowerShell usługi Exchange Online, które obsługują In-Place zbierania elektronicznych materiałów dowodowych i In-Place zbierania elektronicznych materiałów dowodowych. (Te polecenia cmdlet są zbiorczo identyfikowane jako polecenia cmdlet *-MailboxSearch). Obejmuje to następujące polecenia cmdlet:

    - [Nowe wyszukiwanie skrzynek pocztowych](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Polecenie [cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) w programie PowerShell dla usługi Exchange Online.
- Następujące operacje w interfejsie API usług sieci Web programu Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Oś czasu dla wycofania:**
- **1 lipca 2020 r.** Nie możesz już tworzyć nowych wyszukiwań ani blokady, ale możesz uruchamiać, edytować i usuwać istniejące wyszukiwania na własne ryzyko. Pomoc techniczna firmy Microsoft nie obsługuje już In-Place zbierania elektronicznych materiałów dowodowych & eAC.
    
- **1 października 2020** rIn-Place funkcja zbierania elektronicznych materiałów dowodowych & w Aplikacji EAC zostanie umieszczona w trybie tylko do odczytu, więc można tylko usuwać istniejące wyszukiwania i blokady.

**Aby uzyskać więcej informacji, zobacz:**

 - [Migrowanie starszych wyszukiwań i funkcji zbierania elektronicznych materiałów dowodowych do Centrum zgodności platformy Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Wycofanie starszych narzędzi zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Często zadawane pytania dotyczące zbierania In-Place eDiscovery i zbierania elektronicznych In-Place zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




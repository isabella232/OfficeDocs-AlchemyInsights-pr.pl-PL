---
title: Wycofywanie starszych narzędzi zbierania elektronicznych materiałów dowodowych
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
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157668"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Wycofywanie starszych narzędzi zbierania elektronicznych materiałów dowodowych

W wyniku nowej i ulepszonej funkcji zbierania elektronicznych materiałów dowodowych w Centrum zgodności usługi Microsoft 365 następujące starsze narzędzia i polecenia zbierania elektronicznych materiałów dowodowych zostaną wycofane w nadchodzących miesiącach:

- [Zbieranie elektronicznych materiałów dowodowych](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i [blokad y w miejscu](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) w centrum administracyjnym programu Exchange.

- Polecenia cmdlet programu Exchange Online PowerShell obsługujące zbieranie elektronicznych materiałów dowodowych i blokady w miejscu. (Te polecenia cmdlet są zbiorczo identyfikowane jako polecenia cmdlet *-MailboxSearch). Obejmuje to następujące polecenia cmdlet:

    - [Wyszukiwanie w nowej skrzynce pocztowej](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Wyszukiwanie skrzynki pocztowej stop](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Polecenie cmdlet [search-mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) w programie Exchange Online PowerShell.
- Następujące operacje w interfejsie API usług sieci Web programu Exchange:
    - [GetSearchableSkrzynki pocztowe](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnSkrzynki pocztowe](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnSkrzynki pocztowe](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Zaawansowane zbieranie elektronicznych materiałów dowodowych usługi Office 365 w 1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Harmonogram przejścia na emeryturę**:
- 1 kwietnia 2020 r.: nie będziesz mieć możliwości tworzenia nowych wyszukiwań i blokad, ale nadal możesz uruchamiać, edytować i usuwać istniejące wyszukiwania na własne ryzyko. Pomoc techniczna firmy Microsoft nie będzie już obsługiwać & w eAC w miejscu zbierania &.

- 1 lipca 2020 r.: Funkcja wykrywania & w miejscu w eAC zostanie umieszczona w trybie tylko do odczytu. Oznacza to, że możesz usuwać tylko istniejące wyszukiwania i blokady.

**Aby uzyskać więcej informacji, zobacz:**

 - [Migrowanie starszych wyszukiwań zbierania elektronicznych materiałów dowodowych i blokad do centrum zgodności usługi Microsoft 365](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Wycofywanie starszych narzędzi zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Często zadawane pytania dotyczące zbierania elektronicznych materiałów dowodowych i blokad w miejscu](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




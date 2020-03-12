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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600389"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Wycofywanie starszych narzędzi zbierania elektronicznych materiałów dowodowych

W wyniku nowej i ulepszonej funkcji zbierania elektronicznych materiałów dowodowych w centrum zgodności usługi Microsoft 365 w nadchodzących miesiącach zostaną wycofane następujące starsze narzędzia i polecenia zbierania elektronicznych materiałów dowodowych:

- [W miejscu zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i [blokad miejscowych](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) w centrum administracyjnym programu Exchange.

- Polecenia cmdlet programu Exchange Online programu PowerShell obsługujące zbieranie elektronicznych materiałów dowodowych i blokady miejscowe. (Te polecenia cmdlet są zbiorczo identyfikowane jako polecenia cmdlet *-MailboxSearch). Obejmuje to następujące polecenia cmdlet:

    - [Wyszukiwanie skrzynki pocztowej](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Wyszukiwanie skrzynki pocztowej start](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Wyszukiwanie skrzynki pocztowej](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Wyszukiwanie skrzynki pocztowej](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Polecenie cmdlet [Skrzynki wyszukiwania](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) w programie Exchange Online PowerShell.
- Następujące operacje w interfejsie API usług sieci Web programu Exchange:
    - [GetSearchableSkrzynki pocztowe](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnSkrzynki pocztowe](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Skrzynki pocztowe GetHoldOn](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Zaawansowane zbieranie elektronicznych materiałów dowodowych usługi Office 365 w 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Harmonogram przejścia na emeryturę**:
- Kwiecień 1, 2020: Nie będziesz mógł tworzyć nowych wyszukiwań i blokad, ale nadal możesz uruchamiać, edytować i usuwać istniejące wyszukiwania na własne ryzyko. Pomoc techniczna firmy Microsoft nie będzie już obsługiwać zbierania elektronicznych materiałów dowodowych & w witrynie EAC.

- 1 lipca 2020 r.: Funkcja zbierania elektronicznych materiałów dowodowych & w trybie EAC zostanie umieszczona w trybie tylko do odczytu. Oznacza to, że możesz usuwać tylko istniejące wyszukiwania i blokady.

**Aby uzyskać więcej informacji, zobacz:**

 - [Migrowanie starszych wyszukiwań zbierania elektronicznych materiałów dowodowych i blokad do centrum zgodności usługi Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Wycofywanie starszych narzędzi zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Często zadawane pytania dotyczące zbierania elektronicznych materiałów dowodowych i blokad w miejscu](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




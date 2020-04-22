---
title: Wycofanie starszych narzędzi zbierania elektronicznych materiałów dowodowych
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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650578"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Wycofanie starszych narzędzi zbierania elektronicznych materiałów dowodowych

W wyniku nowych i ulepszonych funkcji zbierania elektronicznych materiałów dowodowych w Centrum zgodności usługi Microsoft 365 następujące starsze narzędzia zbierania elektronicznych materiałów dowodowych i polecenia zostaną wycofane w nadchodzących miesiącach:

- [Zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) w miejscu i [blokad w miejscu](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) w centrum administracyjnym programu Exchange.

- Polecenia cmdlet programu Exchange Online PowerShell obsługujące elektroniczne zbierania elektronicznych materiałów dowodowych w miejscu i w miejscu. (Te polecenia cmdlet są zbiorczo identyfikowane jako polecenia cmdlet *-MailboxSearch). Obejmuje to następujące polecenia cmdlet:

    - [Nowa skrzynka pocztowaWyszukuj](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Uruchamianie skrzynki pocztowejWyszukuj](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Zatrzymaj Skrzynkę pocztowąWyszukuj](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-Skrzynka pocztowaWyszukuj](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Polecenie cmdlet [skrzynki pocztowej wyszukiwania](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) w programie Exchange Online PowerShell.
- Następujące operacje w interfejsie API usług sieci Web programu Exchange:
    - [Skrzynki Odbiorcze GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Skrzynki SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Skrzynki GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Zaawansowane funkcje zbierania elektronicznych materiałów dowodowych w wersji 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Harmonogram przejścia na emeryturę:**
- 1 kwietnia 2020 r.: nie będzie można tworzyć nowych wyszukiwań i blokad, ale nadal możesz uruchamiać, edytować i usuwać istniejące wyszukiwania na własne ryzyko. Pomoc techniczna firmy Microsoft nie będzie już obsługiwać blokad zbierania elektronicznych materiałów dowodowych w miejscu & w eAC.

- 1 lipca 2020 r.: Funkcja zbierania elektronicznych materiałów dowodowych w miejscu & w EAC zostanie umieszczona w trybie tylko do odczytu. Oznacza to, że możesz usuwać tylko istniejące wyszukiwania i blokady.

**Aby uzyskać więcej informacji, zobacz**:

 - [Migrowanie starszych wyszukiwań zbierania elektronicznych materiałów dowodowych i blokad do centrum zgodności usługi Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Wycofanie starszych narzędzi zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Często zadawane pytania dotyczące zbierania elektronicznych materiałów dowodowych w miejscu i blokad w miejscu](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




---
title: Chcesz oznaczyć bezpieczną domenę lub nadawcę poczty e-mail?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281181"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Chcesz oznaczyć bezpieczną domenę lub nadawcę poczty e-mail?

- Korzystanie z **list bezpiecznych nadawców nie jest zalecane,** ponieważ otwiera organizację na ataki spamowe, phish i spoofing.
- Jeśli jednak istnieje wymóg biznesowy, **zalecamy** użycie w tym celu **[reguł przepływu poczty.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Nasze wskazówki zapewniają uwierzytelnianie nadawcy (weryfikuje, że domena wysyłająca nie jest sfałszowana). **Uwaga:** Nie zalecamy zarządzania fałszywymi alarmami przy użyciu list bezpiecznych nadawców, ponieważ wyjątki od filtrowania spamu mogą otworzyć twoją organizację na ataki zabezpieczeń. Jeśli użytkownicy odbierają wiadomości niepoprawnie oznaczone jako spam lub wiadomości-śmieci, **[zgłoś wiadomości i pliki firmie Microsoft.](https://protection.office.com/reportsubmission)**
- Należy unikać bezpiecznych nadawców w programie Outlook, listy dozwolonych nadawców lub listy dozwolonych domen w zasadach **antyspamowych,** ponieważ nadawcy omijają wszelką ochronę przed spamem, fałszem i phish oraz uwierzytelnianie nadawców (SPF, DKIM, DMARC). Ta metoda jest najlepiej używana tylko do testowania tymczasowego.

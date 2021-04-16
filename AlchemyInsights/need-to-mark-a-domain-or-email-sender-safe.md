---
title: Chcesz oznaczyć bezpieczną domenę lub nadawcę poczty e-mail?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792142"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Chcesz oznaczyć bezpieczną domenę lub nadawcę poczty e-mail?

- Korzystanie z **list bezpiecznych nadawców** nie jest zalecane, ponieważ otwiera organizację na spam, wyłudzy i spoofing.
- Jeśli jednak istnieją wymagania biznesowe, zalecamy używanie **w tym** celu reguł **[przepływu](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** poczty. Nasze wskazówki zapewniają, że uwierzytelnianie nadawcy (sprawdza, czy wysyłanie domeny nie jest sfałszowane). **Uwaga:** Nie zalecamy zarządzania wyników fałszywie dodatnich za pomocą list bezpiecznych nadawców, ponieważ wyjątki od filtrowania spamu mogą otworzyć Twoją organizację na ataki zabezpieczeń. Jeśli Twoi użytkownik otrzymuje wiadomości nieprawidłowo oznaczone jako spam lub wiadomości-śmieci, zgłoś te wiadomości **[i pliki do firmy Microsoft.](https://protection.office.com/reportsubmission)**
- Należy unikać stosowania zasad bezpiecznych nadawców w programie  Outlook, listy dozwolonych nadawców lub listy domen dozwolonych w zasadach ochrony przed spamem, ponieważ nadawcy pomijają całą ochronę przed spamem, fałszem i wyłudzką oraz uwierzytelnianie nadawców (SPF, DKIM, DMARC). Ta metoda jest najlepsza w przypadku tylko testów tymczasowych.

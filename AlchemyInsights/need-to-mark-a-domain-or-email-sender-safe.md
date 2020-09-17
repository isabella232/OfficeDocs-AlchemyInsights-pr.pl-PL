---
title: Chcesz bezpiecznie oznaczyć domenę lub nadawcę wiadomości e-mail?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803255"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Chcesz bezpiecznie oznaczyć domenę lub nadawcę wiadomości e-mail?

- Korzystanie z **list bezpiecznych nadawców nie jest zalecane** , ponieważ powoduje otwarcie organizacji na ataki z spamem, phishingiem i fałszowaniem.
- Jeśli jednak istnieje wymóg biznesowy, **zalecamy** korzystanie z **[reguł przepływu poczty](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** . Nasze wskazówki gwarantują uwierzytelnienie nadawcy (sprawdzanie, że domena wysłana nie jest fałszywa). **Uwaga**: nie zalecamy zarządzania fałszywymi wynikami pozytywnymi przy użyciu list bezpiecznych nadawców, ponieważ wyjątki dotyczące filtrowania spamu mogą otwierać organizację w celu zapewnienia bezpieczeństwa. Jeśli użytkownik otrzyma wiadomości niepoprawnie oznaczone jako spam lub wiadomości-śmieci, prosimy **[o zgłoszenie wiadomości i plików do firmy Microsoft](https://protection.office.com/reportsubmission)**.
- **Można uniknąć** bezpiecznych nadawców w programie Outlook, listy dozwolonych nadawców lub listy dozwolonych domen w zasadach ochrony przed spamem, ponieważ nadawcy pomijają wszystkie spam, fałszowanie i ochronę przed wirusami oraz uwierzytelnianie nadawcy (SPF, DKIM, DMARC). Ta metoda jest najbardziej przydatna tylko w przypadku tymczasowych testów.

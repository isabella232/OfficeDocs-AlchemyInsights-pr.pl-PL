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
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286690"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Chcesz oznaczyć bezpieczną domenę lub nadawcę poczty e-mail?

- Korzystanie z **list bezpiecznych nadawców** nie jest zalecane, ponieważ otwiera organizację na spam, wyłudzy i spoofing.
- Jeśli jednak istnieją wymagania biznesowe, **zalecamy** używanie w tym celu reguł poczty **[Flow poczty.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Nasze wskazówki zapewniają, że uwierzytelnianie nadawcy (sprawdza, czy wysyłanie domeny nie jest sfałszowane). **Uwaga:** Nie zalecamy zarządzania wyników fałszywie dodatnich za pomocą list bezpiecznych nadawców, ponieważ wyjątki od filtrowania spamu mogą otworzyć Twoją organizację na ataki zabezpieczeń. Jeśli Twoi użytkownik otrzymuje wiadomości nieprawidłowo oznaczone jako spam lub wiadomości-śmieci, zgłoś te wiadomości **[i pliki do firmy Microsoft.](https://protection.office.com/reportsubmission)**
- Sejf Należy unikać stosowania Outlook nadawców z listy dozwolonych nadawców  lub listy dozwolonych domen w zasadach ochrony przed spamem, ponieważ nadawcy pomijają całą ochronę przed spamem, fałszem i wyłudkiem oraz uwierzytelnianie nadawców (SPF, DKIM, DMARC). Ta metoda jest najlepsza w przypadku tylko testów tymczasowych.
- Sprawdzanie poprawności, czy określone wiadomości e-mail pomijały sprawdzanie ochrony przed spamem, można sprawdzić, sprawdzając nagłówek wiadomości "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SN), zobacz Nagłówki wiadomości ochrony przed **[spamem.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Firma Microsoft chce, aby klienci domyślnie [zadbali](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)o bezpieczeństwo swoich klientów, dlatego niektóre zmiany w dzierżawie nie są stosowane do złośliwego oprogramowania ani do wyłudzania dużej pewności. Obejmują one: listy dozwolonych nadawców lub listy dozwolonych domen (zasady ochrony przed spamem) o Outlook Sejf o Lista dozwolonych adresów IP nadawców (filtrowanie połączeń) 
- Jedynym zastępowaniem pozwalającym na pominięcie filtrowania wiadomości służącej do wyłudzania informacji o wysokiej pewności jest pominięcie Exchange przepływu poczty (nazywane także regułami transportu). Aby użyć reguł przepływu poczty e-mail w celu obejścia filtrowania, zobacz Ustawianie poziomu ufności **[filtru spamu (SCL)](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)** w wiadomościach za pomocą reguł przepływu poczty.
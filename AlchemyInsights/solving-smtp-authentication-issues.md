---
title: Włączanie uwierzytelniania SMTP i rozwiązywania problemów
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
- "3000003"
- "5652"
ms.openlocfilehash: d16389ca577970deaf743255f75dc86134e79dcab2fff8c33987532fc7ee1105
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890444"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Włączanie uwierzytelniania SMTP i rozwiązywania problemów

Jeśli chcesz włączyć uwierzytelnianie SMTP dla skrzynki pocztowej lub jest wyświetlany komunikat o błędzie "Nie można uwierzytelnić klienta", "Uwierzytelnienie nie powiodło się" lub "SmtpClientAuthentication" z kodem 5.7.57 albo 5.7.3 lub 5.7.139 podczas próby przekazywania wiadomości e-mail przez uwierzytelnienie urządzenia lub aplikacji przy użyciu programu Microsoft 365, wykonaj następujące trzy czynności, aby rozwiązać ten problem:

1. Wyłącz domyślne [ustawienia zabezpieczeń platformy Azure,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) przełączanie opcji Włącz **domyślne ustawienia zabezpieczeń** na **Nie.**

    a. Zaloguj się do portalu Azure jako administrator zabezpieczeń, administrator dostępu warunkowego lub administrator globalny.<BR/>
    b. Przejdź do Azure Active Directory > **Właściwości.**<BR/>
    c. Wybierz **pozycję Zarządzaj ustawieniami domyślnymi zabezpieczeń.**<BR/>
    d. Ustaw **wartość Włącz domyślne ustawienia zabezpieczeń** na **Nie**.<BR/>
    e. Wybierz **Zapisz**.

2. [Włącz przesyłanie smtp klienta](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) dla licencjonowanej skrzynki pocztowej.

    a. W centrum administracyjne platformy Microsoft 365 przejdź do **strony Aktywni użytkownicy** i wybierz użytkownika.<BR/>
    b. Przejdź do karty Poczta, a następnie w obszarze **Aplikacje poczty e-mail** wybierz **pozycję Zarządzaj aplikacjami poczty e-mail**.<BR/>
    d. Upewnij **się, że jest zaznaczona** opcja Uwierzytelniony SMTP (włączona).<BR/>
    e. Wybierz **pozycję Zapisz zmiany.**<BR/>

3. [Wyłącz uwierzytelnianie wieloskładnikowe (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) dla licencjonowanej skrzynki pocztowej.

    a. Przejdź do centrum administracyjne platformy Microsoft 365 i w menu nawigacji po lewej stronie wybierz **pozycję Użytkownicy**  >  **Aktywni użytkownicy.**<BR/>
    b. Wybierz **pozycję Uwierzytelnianie wieloskładnikowe.**<BR/>
    c. Wybierz użytkownika i wyłącz **funkcję Multi-Factor Auth.**<BR/>

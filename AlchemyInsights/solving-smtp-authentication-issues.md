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
ms.openlocfilehash: f6f0228f6cdf7e07c9f439c54a7a2bd5364381c0e47dc80117bd964c5eafea61
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957218"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Włączanie uwierzytelniania SMTP i rozwiązywania problemów

Jeśli chcesz włączyć uwierzytelnianie SMTP dla skrzynki pocztowej lub jest wyświetlany komunikat o błędzie "Klient nie uwierzytelniony", "Uwierzytelnienie nie powiodło się" lub "SmtpClientAuthentication" z kodem 5.7.57 albo 5.7.3 lub 5.7.139 podczas próby przekazywania wiadomości e-mail przez uwierzytelnienie urządzenia lub aplikacji przy użyciu programu Microsoft 365, wykonaj następujące trzy czynności, aby rozwiązać ten problem:

1. Wyłącz domyślne [ustawienia zabezpieczeń platformy Azure,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) przełączanie opcji Włącz **domyślne ustawienia zabezpieczeń** na **Wartość Nie.**

    a. Zaloguj się do portalu Azure jako administrator zabezpieczeń, administrator dostępu warunkowego lub administrator globalny.<BR/>
    b. Przejdź do Azure Active Directory > **właściwości.**<BR/>
    c. Wybierz **pozycję Zarządzaj ustawieniami domyślnymi zabezpieczeń.**<BR/>
    d. Ustaw **wartość Włącz domyślne ustawienia zabezpieczeń** na **Nie**.<BR/>
    e. Wybierz **Zapisz**.

2. [Włącz przesyłanie smtp klienta](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) dla licencjonowanej skrzynki pocztowej.

    a. Z centrum administracyjne platformy Microsoft 365 przejdź do **strony Aktywni użytkownicy** i wybierz użytkownika.<BR/>
    b. Przejdź do karty Poczta, a następnie w obszarze **Aplikacje poczty e-mail** wybierz **pozycję Zarządzaj aplikacjami poczty e-mail**.<BR/>
    d. Upewnij **się, że jest zaznaczona** opcja Uwierzytelniony SMTP (włączona).<BR/>
    e. Wybierz **pozycję Zapisz zmiany.**<BR/>

3. [Wyłącz uwierzytelnianie wieloskładnikowe (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) dla licencjonowanej skrzynki pocztowej.

    a. Przejdź do centrum administracyjne platformy Microsoft 365, a następnie w lewym menu nawigacji wybierz **pozycję**  >  **Aktywni użytkownicy** Użytkownicy.<BR/>
    b. Wybierz **pozycję Uwierzytelnianie wieloskładnikowe**.<BR/>
    c. Wybierz użytkownika i wyłącz **funkcję Multi-Factor Auth.**<BR/>

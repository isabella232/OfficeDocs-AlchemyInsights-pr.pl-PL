---
title: 451 4.7.0 Błąd serwera tymczasowego. Spróbuj ponownie później. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812586"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Błąd serwera tymczasowego. Spróbuj ponownie później. PRX4

Podczas wysyłania wiadomości e-mail za pośrednictwem witryny Smarthost "smtp.office365.com" przy użyciu metody przesyłania klienta SMTP może wystąpić błąd: "451 4.7.0 Błąd serwera tymczasowego". Spróbuj ponownie później. PRX4 ma przeważnie charakter tymczasowy". 

Upewnij się, że nie używasz udostępnionej skrzynki pocztowej do przesyłania klienta SMTP, ponieważ metoda przesyłania klienta SMTP wymaga licencjonowanej skrzynki pocztowej do wysyłania poczty za jej pośrednictwem. Jeśli jednak nie korzystasz z udostępnionej skrzynki pocztowej i problem będzie nadal występował, sprawdź następujące kwestie:

1. Włącz przesyłanie SMTP klienta na licencjonowanej skrzynce pocztowej używanej przez uruchomienie tego polecenia programu PowerShell:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    LUB

    1. Przejdź do centrum administracyjne platformy Microsoft 365 > **aktywni użytkownicy,** a następnie wybierz użytkownika.
    1. Przejdź do karty Poczta, > **pozycję Aplikacje poczty e->** pozycję Zarządzaj aplikacjami **poczty e-mail.** 
    1. Upewnij się, że jest zaznaczone (włączone) ustawienie **Uwierzytelnione SMTP.**
    1. Wybierz **pozycję Zapisz zmiany.**
    
    Aby włączyć uwierzytelnianie SMTP w całej organizacji, uruchom to polecenie:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Uwaga:** Ze względów bezpieczeństwa zalecane jest włączenie uwierzytelniania SMTP tylko dla używanej skrzynki pocztowej. Ustawienie na poziomie użytkownika zastępuje ustawienie na poziomie organizacji.

2. Wyłącz ustawienia domyślne zabezpieczeń platformy Azure, przełączanie wartości **Domyślnych ustawień zabezpieczeń na** **Nie:**

    1. Zaloguj się do portalu Azure jako administrator zabezpieczeń, administrator dostępu warunkowego lub administrator globalny.
    1. Przejdź do Azure Active Directory >**  zabezpieczeń** i wybierz **pozycję Zarządzaj domyślnymi ustawieniami zabezpieczeń.**
    1. Ustaw przełącznik **Włącz domyślne ustawienia zabezpieczeń** na **Nie**.
    1. Wybierz **Zapisz**.

3. Wyłącz uwierzytelnianie wieloskładnikowe (MFA) dla licencjonowanej skrzynki pocztowej, która jest używana.

    1. Przejdź do centrum administracyjne platformy Microsoft 365, a następnie w lewym menu nawigacji wybierz pozycję **Użytkownicy**  >  **Aktywni użytkownicy.**
    1. Na stronie **Aktywni użytkownicy** wybierz pozycję **Uwierzytelnianie wieloskładnikowe**.
    1. Wybierz użytkownika i wyłącz **uwierzytelnianie wieloskładnikowe.**


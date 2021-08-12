---
title: Czy użytkownicy otrzymali złośliwą wiadomość e-mail?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929207"
---
# <a name="did-your-users-receive-malicious-email"></a>Czy użytkownicy otrzymali złośliwą wiadomość e-mail?

- Teraz możesz zgłosić złośliwą wiadomość e-mail do firmy Microsoft za pomocą opcji [Przesłane zgłoszenia przez administratorów w Centrum zabezpieczeń i zgodności](https://sip.protection.office.com/reportsubmission).

Wiadomości przesłane w obszarze [przesłane zgłoszenia przez administratorów](https://sip.protection.office.com/reportsubmission) są skanowane, a następujące wyniki są wyświetlane w menu wysuwanym **szczegółów**:

- Jeśli wystąpił błąd w uwierzytelnianiu wiadomości e-mail nadawcy w czasie dostarczania.
- Informacje na temat wskazówek dotyczących zasad, które mogły wpłynąć na werdykt wiadomości lub go pominąć.
- Bieżące wyniki detonacji, aby sprawdzić, czy adresy URL lub pliki zawarte w wiadomości były złośliwe.
- Informacja zwrotna od mechanizmów oceniających

Jeśli wykryto pominięcie, ponowne skanowanie powinno zostać zakończone w ciągu kilku minut. Jeśli w uwierzytelnianiu wiadomości e-mail nie wystąpił błąd, bądź pominięcie nie miało wpływu na dostarczenie, wtedy uzyskanie informacji zwrotnej od mechanizmów oceniających może zająć nawet jeden dzień.

Jeśli nie zgadzasz się z ostatecznym werdyktem dotyczącym wiadomości, adresu URL lub pliku (zablokowany lub niezablokowany), prześlij ponownie wiadomość po upływie jednego dnia w celu wykonania ponownego skanowania. Istnieje wysokie prawdopodobieństwo, że werdykt może ulec zmianie po ponownym przesłaniu wiadomości.

W międzyczasie możesz usunąć złośliwą wiadomość e-mail ze skrzynek odbiorczych użytkowników, wykonując czynności opisane w [tym artykule](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Klienci w ramach ochrony usługi Office 365 w usłudze Microsoft Defender mogą:
    - użyć [eksploratora zagrożeń w celu znalezienie i usunięcia podejrzanej wiadomości e-mail](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [użyć bezpiecznych linków do zablokowania dostępu](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) do złośliwego adresu URL
    - śledzić użytkowników, którzy kliknęli i uzyskali dostęp do złośliwych adresów URL: [wyświetl adres URL wyłudzający informacje i kliknij dane dotyczące werdyktu](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - ręcznie[uruchomić zautomatyzowane badanie](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Możesz też zabezpieczyć się przed złośliwymi plikami i adresami URL, wykonując czynności opisane w artykule [Ochrona przed złośliwymi adresami URL i plikami](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
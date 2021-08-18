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
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326713"
---
# <a name="did-your-users-receive-malicious-email"></a>Czy użytkownicy otrzymali złośliwą wiadomość e-mail?

Teraz możesz zgłosić złośliwą wiadomość e-mail do firmy Microsoft [za pomocą Przesyłania w Microsoft 365 Defender sieci.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Wiadomości przesłane przez [administratorów są](https://security.microsoft.com/reportsubmission?viewid=admin) skanowane i wyświetlane w wysuwanych szczegółach są wyświetlane następujące wyniki:

- Jeśli wystąpił błąd w uwierzytelnianiu wiadomości e-mail nadawcy w czasie dostarczania.
- Informacje na temat wskazówek dotyczących zasad, które mogły wpłynąć na werdykt wiadomości lub go pominąć.
- Bieżące wyniki detonacji, aby sprawdzić, czy adresy URL lub pliki zawarte w wiadomości były złośliwe.
- Informacja zwrotna od mechanizmów oceniających

Jeśli wykryto pominięcie, ponowne skanowanie powinno zostać zakończone w ciągu kilku minut. Jeśli w uwierzytelnianiu wiadomości e-mail nie wystąpił błąd, bądź pominięcie nie miało wpływu na dostarczenie, wtedy uzyskanie informacji zwrotnej od mechanizmów oceniających może zająć nawet jeden dzień.

Jeśli nie zgadzasz się z ostatecznym werdyktem dotyczącym wiadomości, adresu URL lub pliku (zablokowany lub niezablokowany), prześlij ponownie wiadomość po upływie jednego dnia w celu wykonania ponownego skanowania. Istnieje wysokie prawdopodobieństwo, że werdykt może ulec zmianie po ponownym przesłaniu wiadomości.

W międzyczasie możesz usunąć złośliwą wiadomość e-mail ze skrzynek odbiorczych użytkowników, wykonując czynności opisane w [tym artykule](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Klienci w ramach ochrony usługi Office 365 w usłudze Microsoft Defender mogą:
  - Znajdowanie [i usuwanie podejrzanych wiadomości e-mail za pomocą Eksploratora zagrożeń](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Blokowanie Sejf dostępu do złośliwego adresu URL za](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) pomocą linków do stron internetowych
  - Śledzenie użytkowników, którzy kliknął i uzyskał dostęp do złośliwych adresów URL: Wyświetlanie adresu URL wyłudzania informacji i [klikanie werdyktowych danych](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Ręczne uruchamianie [automatycznego badania](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Możesz też zabezpieczyć się przed złośliwymi plikami i adresami URL, wykonując czynności opisane w artykule [Ochrona przed złośliwymi adresami URL i plikami](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).

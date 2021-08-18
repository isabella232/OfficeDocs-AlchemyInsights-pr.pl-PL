---
title: Identyfikowanie zewnętrznego przesyłania dalej wiadomości e-mail w skrzynkach pocztowych w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2af731bc9a1e28e2db7c6662041b930e1b05be4c3bf8340784d9ab87101c44af
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899894"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Określanie, kiedy w skrzynkach pocztowych skonfigurowano zewnętrzne przesyłanie dalej poczty e-mail

Gdy użytkownik Microsoft 365 skonfiguruje przesyłanie dalej zewnętrznych wiadomości e-mail w skrzynce pocztowej, działanie jest insektowane w ramach polecenia cmdlet **Set-Mailbox.** Możesz zobaczyć to działanie za pomocą przeszukiwania dziennika inspekcji. Poniżej opisano, jak to zrobić.

1. Wykonaj jedną z następujących czynności:
   - Na stronie Centrum zgodności platformy Microsoft 365 <https://compliance.microsoft.com> przejdź do **tematu Inspekcja** \> **rozwiązań.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://compliance.microsoft.com/auditlogsearch> .
   - W portalu Microsoft 365 Defender w <https://security.microsoft.com> witrynie przejdź do tematu **Inspekcja**. Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://sip.security.microsoft.com/auditlogsearch> .

2. Na stronie **Inspekcja** sprawdź, czy jest **zaznaczona** karta Wyszukiwanie, a następnie skonfiguruj następujące ustawienia:
   - Zaznacz zakres dat i godzin w **polach Rozpoczęcie** **i** Koniec.
   - Sprawdź, **czy pole Działania** zawiera pole Pokaż wyniki dla wszystkich **działań.**

3. Po zakończeniu kliknij pozycję **Wyszukaj**. Działania zostaną wyświetlone na nowej **stronie Przeszukiwanie** inspekcji.

4. W wynikach kliknij pozycję **Filtruj wyniki** i wpisz **Set-Mailbox** w polu filtru aktywności.

5. Zaznacz rekord inspekcji w wynikach. W **wysuwanych** szczegółach kliknij pozycję **Więcej informacji.** Aby ustalić, czy dane działanie jest związane z przesyłaniem dalej poczty e-mail, należy przyjrzeć się szczegółom każdego rekordu inspekcji.

   - **ObjectId:** wartość aliasu zmodyfikowanej skrzynki pocztowej.
   - **Parametry:** _ForwardingSmtpAddress_ wskazuje docelowy adres e-mail.
   - **UserId**: Użytkownik, który skonfigurował przesyłanie dalej poczty e-mail w skrzynce pocztowej w polu **ObjectId.**

Aby uzyskać więcej informacji, zobacz Określanie, kto s skonfigurować [przesyłanie dalej poczty e-mail dla skrzynki pocztowej.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)

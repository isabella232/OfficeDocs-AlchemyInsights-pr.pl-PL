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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028757"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Określanie, kiedy w skrzynkach pocztowych skonfigurowano zewnętrzne przesyłanie dalej poczty e-mail

Gdy użytkownik Microsoft 365 konfiguruje w skrzynce pocztowej zewnętrzne przesyłanie dalej wiadomości e-mail, działanie jest insektowane w ramach polecenia cmdlet **Set-Mailbox.** Możesz zobaczyć działanie za pomocą przeszukiwania dziennika inspekcji w Centrum zabezpieczeń & zgodności.

1. Zaloguj się do [centrum Microsoft 365 zgodności.](https://protection.office.com/)

2. Przejdź do **strony Przeszukiwanie**  >  **dziennika inspekcji wyszukiwania.**

3. Zaznacz zakres dat w **polach Data rozpoczęcia** **i Data zakończenia.** Nie musisz określać nazwy użytkownika. Sprawdź, **czy pole Działania** ma ustawioną wartość Pokaż wyniki dla wszystkich **działań.**

4. Kliknij **przycisk Wyszukaj**.

W wynikach kliknij pozycję **Filtruj wyniki** i wpisz **Set-Mailbox** w polu filtru aktywności. Zaznacz rekord inspekcji w wynikach. W **wysuwanych** szczegółach kliknij pozycję **Więcej informacji.** Aby ustalić, czy dane działanie jest związane z przesyłaniem dalej poczty e-mail, należy przyjrzeć się szczegółom każdego rekordu inspekcji.

- **ObjectId:** wartość aliasu zmodyfikowanej skrzynki pocztowej.

- **Parametry:** _ForwardingSmtpAddress_ wskazuje docelowy adres e-mail.

- **UserId**: Użytkownik, który skonfigurował przesyłanie dalej poczty e-mail w skrzynce pocztowej w polu **ObjectId.**

Aby uzyskać więcej informacji, zobacz Określanie, kto s skonfigurować [przesyłanie dalej poczty e-mail dla skrzynki pocztowej.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)

---
title: Identyfikowanie zewnętrznego przekazywania wiadomości e-mail w skrzynkach pocztowych w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508962"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identyfikowanie, kiedy zewnętrzna przekazywanie poczty e-mail jest skonfigurowane w skrzynkach pocztowych

Gdy użytkownik usługi Microsoft 365 konfiguruje zewnętrzne przekazywanie wiadomości e-mail w skrzynce pocztowej, działanie jest poddane inspekcji w ramach polecenia cmdlet **Set-Mailbox.** Działanie można zobaczyć przy użyciu wyszukiwania dziennika inspekcji w Centrum zgodności & zabezpieczeń.

1. Zaloguj się do [Centrum zgodności & zabezpieczeń usługi Microsoft 365](https://protection.office.com/).

2. Przejdź do **Search**strony wyszukiwania dziennika  >  **inspekcji** wyszukiwania.

3. Wybierz zakres dat w polach **Data rozpoczęcia** i **Data zakończenia.** Nie musisz podawać nazwy użytkownika. Sprawdź, czy pole **Działania** jest ustawione **na Pokaż wyniki dla wszystkich działań**.

4. Kliknij **pozycję Wyszukaj**.

W wynikach kliknij pozycję **Filtruj wyniki** i wpisz **ustaw skrzynkę pocztową** w polu filtru aktywności. Wybierz rekord inspekcji w wynikach. W wysu **nakreślenia szczegółów** kliknij pozycję **Więcej informacji**. Musisz spojrzeć na szczegóły każdego rekordu inspekcji, aby ustalić, czy działanie jest związane z przekazywaniem wiadomości e-mail.

- **ObjectId**: Wartość aliasu zmodyfikowanej skrzynki pocztowej.

- **Parametry**: _ForwardingSmtpAddress_ wskazuje docelowy adres e-mail.

- **Identyfikator użytkownika:** Użytkownik, który skonfigurował przekazywanie wiadomości e-mail w skrzynce pocztowej w polu **ObjectId.**

Aby uzyskać więcej informacji, zobacz [Określanie, kto skonfigurował przekazywanie poczty e-mail dla skrzynki pocztowej](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).

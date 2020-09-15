---
title: Identyfikowanie zewnętrznych przekierowywania wiadomości e-mail dotyczących skrzynek pocztowych w dziennikach inspekcji
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696307"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Określanie, czy w skrzynkach pocztowych jest skonfigurowana zewnętrzna przekierowywanie poczty e-mail

Gdy użytkownik programu Microsoft 365 skonfiguruje zewnętrzną przekierowywanie poczty e-mail w skrzynce pocztowej, działanie jest poddawane inspekcji w ramach polecenia cmdlet **Set-Mailbox** . Działanie można wyświetlić przy użyciu funkcji wyszukiwania dziennika inspekcji w centrum zabezpieczeń & zgodności.

1. Zaloguj się do [Centrum zabezpieczeń & programu Microsoft 365](https://protection.office.com/).

2. Przejdź do strony **Search**  >  **wyszukiwania dziennika inspekcji** wyszukiwania.

3. Wybierz zakres dat w polach **Data rozpoczęcia** i **Data zakończenia** . Nie musisz określać nazwy użytkownika. Upewnij się, że w polu **działania** jest ustawiona wartość **Pokaż wyniki dla wszystkich działań**.

4. Kliknij przycisk **Wyszukaj**.

W wynikach kliknij pozycję **Filtruj wyniki** i wpisz wpis **Set-Skrzynka pocztowa** w polu Filtr aktywności. Wybierz rekord inspekcji w wynikach. W menu wysuwanym **szczegóły** kliknij pozycję **więcej informacji**. Aby określić, czy działanie jest powiązane z przesyłaniem wiadomości e-mail, należy przejrzeć szczegóły każdego rekordu inspekcji.

- **Objectid**: wartość aliasu skrzynki pocztowej, która została zmodyfikowana.

- **Parametry**: _ForwardingSmtpAddress_ wskazuje docelowy adres e-mail.

- **UserID**: użytkownik, który skonfigurował przesyłanie dalej wiadomości e-mail w skrzynce pocztowej w polu **objectid** .

Aby uzyskać więcej informacji, zobacz [Określanie, kto konfiguruje przekierowywanie poczty e-mail dla skrzynki pocztowej](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).

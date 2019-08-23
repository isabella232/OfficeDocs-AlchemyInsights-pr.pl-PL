---
title: Identyfikowanie przekazywanie poczty zewnętrznej skrzynek pocztowych w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539111"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Określenie, jeśli skonfigurowano przesyłanie dalej poczty e-mail zewnętrznej skrzynek pocztowych

Gdy użytkownika w usłudze Office 365 konfiguruje przekazywania zewnętrznych wiadomości e-mail w skrzynce pocztowej, działania jest różna w ramach apletu polecenia **Set-Mailbox** . Możesz zobaczyć działanie przy użyciu przeszukiwania dzienników inspekcji w & zabezpieczeń Centrum zgodności.

1. Zaloguj się do [Centrum zgodności Office 365 zabezpieczeń &](https://protection.office.com/).

2. Przejdź do **wyszukiwania** > stronę**przeszukiwania dzienników inspekcji** .

3. Wybierz zakres dat w polach **Data początkowa** i **Data końcowa** . Nie musisz podać nazwę użytkownika. Sprawdź, czy pole **działalności** jest włączona opcja **Pokaż wyniki dla wszystkich działań**.

4. Kliknij przycisk **Wyszukaj**.

W wynikach kliknij przycisk **Filtruj wyniki** i wpisz **Set-Mailbox** w polu Filtr aktywności. Wybierz rekord audytu w wynikach. W menu wysuwane **Szczegóły** kliknij przycisk **więcej informacji**. Należy spojrzeć na szczegóły poszczególnych rekordów inspekcji w celu określenia, jeśli działanie jest powiązane z przekazywanie wiadomości e-mail.

- **Identyfikator obiektu**: wartość alias skrzynki pocztowej, który został zmodyfikowany.

- **Parametry**: _ForwardingSmtpAddress_ wskazuje docelowy adres e-mail.

- **Identyfikator użytkownika**: użytkownik, który skonfigurować przekazywanie poczty e-mail do skrzynki pocztowej w polu **identyfikator obiektu** .

Aby uzyskać więcej informacji zobacz [Określanie, która skonfigurowała przekazywanie dla skrzynki pocztowej wiadomości e-mail](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).

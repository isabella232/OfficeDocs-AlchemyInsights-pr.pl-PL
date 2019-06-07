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
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752027"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Określenie, jeśli skonfigurowano przesyłanie dalej poczty e-mail zewnętrznej skrzynek pocztowych

Gdy użytkownik konfiguruje przekazywania zewnętrznych wiadomości e-mail w skrzynce pocztowej, działania jest różna w ramach apletu polecenia **Set-Mailbox** . Możesz zobaczyć działanie przy użyciu przeszukiwania dzienników inspekcji w & zabezpieczeń Centrum zgodności.

1. Zaloguj się do [Centrum zgodności Office 365 zabezpieczeń &](https://protection.office.com/)

2. Kliknij przycisk **Wyszukaj i dochodzenia** i wybierz **Przeszukiwania dzienników inspekcji**.

3. Wybierz zakres dat w polach **Data początkowa** i **Data końcowa** . Nie musisz podać nazwę użytkownika. Sprawdź, czy pole **działalności** jest włączona opcja **Pokaż wyniki dla wszystkich działań**.

4. Kliknij przycisk **Wyszukaj**.

W wynikach kliknij przycisk **Filtruj wyniki** i wpisz **Set-Mailbox** w polu Filtr aktywności. Wybierz rekord audytu w wynikach. W menu wysuwane **Szczegóły** kliknij przycisk **więcej informacji**. Należy spojrzeć na szczegóły poszczególnych rekordów inspekcji w celu określenia, jeśli działanie jest powiązane z przekazywanie wiadomości e-mail.

- **Identyfikator obiektu**: wartość alias skrzynki pocztowej, który został zmodyfikowany.

- **Parametry**: _ForwardingSmtpAddress_ wskazuje docelowy adres e-mail.

- **Identyfikator użytkownika**: użytkownik, który skonfigurować przekazywanie poczty e-mail do skrzynki pocztowej w polu **identyfikator obiektu** .

Aby uzyskać więcej informacji zobacz [Określanie, która skonfigurowała przekazywanie dla skrzynki pocztowej wiadomości e-mail](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).

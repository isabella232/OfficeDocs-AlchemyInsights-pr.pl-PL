---
title: Rozwiązywanie problemów ze zdarzeniami z poczty e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569408"
---
# <a name="troubleshooting-events-from-email"></a>Rozwiązywanie problemów ze zdarzeniami z poczty e-mail

1. Sprawdź, czy funkcja jest włączona dla skrzynki pocztowej: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Następnie spójrz na "Zdarzenia z wiadomości e-mail" dzienniki **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. W dziennikach "Zdarzenia z wiadomości e-mail" znajdź identyfikator InternetMessageId, który pasuje do elementu w skrzynce pocztowej.  

4. TrustScore określa, czy element jest dodawany, czy nie. Zdarzenia zostaną dodane tylko wtedy, gdy TrustScore = "Trusted".

TrustScore jest określana przez SPF, Dkim lub Dmarc właściwości, które znajdują się w nagłówku wiadomości.

Aby wyświetlić te właściwości:

**Program Outlook dla komputerów stacjonarnych**

- Otwieranie elementu
- Właściwości pliku -> -> nagłówki internetowe

lub

**Mfcmapi**

- Przejdź do elementu w skrzynce odbiorczej
- Poszukaj PR_TRANSPORT_MESSAGE_HEADERS_W

Właściwości te są określane i rejestrowane podczas transportu i routingu. Aby uzyskać dalsze rozwiązywanie problemów, może być konieczne monitorowanie obsługi transportu dotyczące błędów w filtrze SPF, DKIM i.lub DMARC.
---
title: Rozwiązywanie problemów z pocztą E-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658744"
---
# <a name="troubleshooting-events-from-email"></a>Rozwiązywanie problemów z pocztą E-mail

1. Sprawdzanie, czy funkcja jest włączona dla skrzynki pocztowej: **Get-EventsFromEmailConfiguration <mailbox> -Identity**

2. Następnie sprawdź dzienniki "zdarzenia z poczty E-mail" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. W dziennikach "zdarzenia z poczty E-mail" Znajdź InternetMessageId pasujący do elementu w skrzynce pocztowej.  

4. TrustScore określa, czy dany element został dodany, czy nie. Zdarzenia zostaną dodane tylko wtedy, gdy TrustScore = "zaufane".

TrustScore jest określany na podstawie właściwości SPF, DKIM lub DMARC, które znajdują się w nagłówku wiadomości.

Aby wyświetlić te właściwości:

**Program Outlook dla komputerów stacjonarnych**

- Otwórz element
- Plik — właściwości >-> nagłówki internetowe

lub

**MFCMapi**

- Przechodzenie do elementu w skrzynce odbiorczej
- Szukaj PR_TRANSPORT_MESSAGE_HEADERS_W

Te właściwości są określane i rejestrowane podczas transportu i routingu. Aby uzyskać dalsze Rozwiązywanie problemów, może być konieczne wykonanie dodatkowych czynności w zakresie pomocy technicznej transportowej dotyczących błędów w programie SPF, DKIM i. lub DMARC.
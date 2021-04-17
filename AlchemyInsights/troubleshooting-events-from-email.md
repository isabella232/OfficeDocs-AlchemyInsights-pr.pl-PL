---
title: Rozwiązywanie problemów ze zdarzeniami z poczty e-mail
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834849"
---
# <a name="troubleshooting-events-from-email"></a>Rozwiązywanie problemów ze zdarzeniami z poczty e-mail

1. Sprawdzanie, czy funkcja jest włączona dla skrzynki pocztowej: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Następnie przyjrzyj się dziennikom "Zdarzenia z poczty **e-mail" Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. W dziennikach "Events from Email" (Zdarzenia z poczty e-mail) znajdź element InternetMessageId, który odpowiada elementowi w skrzynce pocztowej.  

4. Wartość TrustScore określa, czy element został dodany. Zdarzenia zostaną dodane tylko wtedy, gdy trustScore = "Trusted".

Wartość TrustScore jest określana przez właściwości SPF, Dkim lub Dmarc, które znajdują się w nagłówku wiadomości.

Aby wyświetlić te właściwości:

**Klasyczny program Outlook**

- Otwieranie elementu
- Plik — > właściwości -> nagłówków internetowych

lub

**MFCMapi**

- Przechodzenie do elementu w skrzynce odbiorczej
- Poszukaj PR_TRANSPORT_MESSAGE_HEADERS_W

Te właściwości są określane i rejestrowane podczas transportu i routingu. W celu dalszego rozwiązywania problemów może być konieczne swoicie się z pomocą techniczną transportu w przypadku błędów SPF, DKIM i DMARC.
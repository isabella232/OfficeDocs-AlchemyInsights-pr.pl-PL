---
title: AntiSpam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717335"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail związanych z kodem błędu 5.7.23

Sprawdź rekord SPF DNS dla swojej domeny w publicznie dostępnym narzędziu SPF lub Sprawdzanie rekordów DNS w sieci Web.

Upewnij się, że wiadomość wychodząca nie została zidentyfikowana jako spam przez firmę Microsoft i przekierowana przez [pulę dostarczania wysokiego ryzyka](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Wiadomości w puli dostarczania wysokiego ryzyka nie będą przekazywać testów SPF, więc nie zostaną zaakceptowane przez docelową organizację poczty e-mail.

Jeśli problem będzie nadal występował, może być konieczne skontaktowanie się z administratorem hosta poczty, do którego próbujesz wysłać wiadomość e-mail. Zanotuj szczegółowy błąd zewnętrzny, który jest dostępny w wiadomości odskakującej. Pomoc techniczna firmy Microsoft może nie być w stanie pomóc dalej.

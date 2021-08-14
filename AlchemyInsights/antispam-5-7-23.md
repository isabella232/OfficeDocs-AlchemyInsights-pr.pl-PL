---
title: Ochrona przed spłacami — 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932179"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail związanych z kodem błędu 5.7.23

Zweryfikuj rekord DNS SPF dla swojej domeny w publicznie dostępnym kontrolerze rekordu SPF lub DNS w sieci Web.

Sprawdź, czy wiadomość wychodząca nie została zidentyfikowany przez firmę Microsoft jako spam i przekierowyowana przez pulę dostarczania [wysokiego ryzyka.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Wiadomości w puli dostarczania wysokiego ryzyka nie będą podlegały testom SPF, a zatem nie będą akceptowane przez docelową organizację poczty e-mail.

Jeśli problem będzie nadal występował, może być konieczne skontaktowanie się z administratorem hosta poczty, do którego próbujesz wysłać wiadomość e-mail. Zanotuj szczegółowy błąd zewnętrzny dostępny w wiadomości zwracaowej. Pomoc techniczna firmy Microsoft może nie być w stanie dalej pomóc.

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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821421"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rozwiązywanie problemów dotyczących dostarczania wiadomości e-mail związanych z kodem błędu 5.7.23

Zweryfikuj rekord DNS SPF dla swojej domeny w publicznie dostępnym kontrolerze rekordu SPF lub DNS w sieci Web.

Sprawdź, czy wiadomość wychodząca nie została zidentyfikowany przez firmę Microsoft jako spam i przekierowyowana przez pulę dostarczania [wysokiego ryzyka.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Wiadomości w puli dostarczania wysokiego ryzyka nie będą podlegały testom SPF, a zatem nie będą akceptowane przez docelową organizację poczty e-mail.

Jeśli problem będzie nadal występował, może być konieczne skontaktowanie się z administratorem hosta poczty, do którego próbujesz wysłać wiadomość e-mail. Zanotuj szczegółowy błąd zewnętrzny dostępny w wiadomości zwracaowej. Pomoc techniczna firmy Microsoft może nie być w stanie dalej pomóc.

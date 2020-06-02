---
title: Antyspam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506453"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rozwiązywanie problemów z dostarczaniem wiadomości e-mail dla kodu błędu 5.7.23

Sprawdź rekord DNS SPF dla domeny w publicznie dostępnym kontrolerze SPF lub DNS w sieci Web.

Sprawdź, czy wiadomość wychodząca nie została zidentyfikowana jako spam przez firmę Microsoft i przekierowana przez [pulę dostarczania wysokiego ryzyka.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Wiadomości w puli dostarczania wysokiego ryzyka nie będą przechodzić kontroli SPF i dlatego nie będą akceptowane przez docelową organizację poczty e-mail.

Jeśli problem będzie się powtarzał, może być konieczne skontaktowanie się z administratorem hosta poczty, do którego próbujesz wysłać wiadomość e-mail. Zanotuj szczegółowy błąd zewnętrzny dostępny w komunikacie o odrzuceniu. Pomoc techniczna firmy Microsoft może nie być w stanie pomóc dalej.

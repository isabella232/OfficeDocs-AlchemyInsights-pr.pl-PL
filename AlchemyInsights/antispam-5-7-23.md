---
title: AntiSpam-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682236"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Napraw problemy z dostarczaniem wiadomości e-mail dla kodu błędu 5.7.23

Zweryfikuj rekord SPF DNS dla swojej domeny w publicznie dostępnym kontrolerze rekordów SPF lub DNS w sieci Web.

Sprawdź, czy wiadomość wychodząca nie została zidentyfikowana jako spam przez pakiet Office 365 i kierowane przez [pulę dostawy wysokiego ryzyka](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Wiadomości w puli dostaw wysokiego ryzyka nie przejdzie kontroli SPF i dlatego nie będą akceptowane przez organizację docelową pocztę e-mail.

Jeśli problem będzie się powtarzał, może być konieczne skontaktowanie się z administratorem hosta poczty, do którego próbujesz wysłać wiadomość e-mail. Zanotuj szczegółowy błąd zewnętrzny dostępny w wiadomości odbijanie.  Pomoc techniczna pakietu Office 365 może nie być w stanie udzielić dalszej pomocy.
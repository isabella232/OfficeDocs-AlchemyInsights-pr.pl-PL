---
title: Wystąpił błąd sprawdzania poprawności tokenu dostępu podczas wnoszania analizy komputerowej
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
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946625"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Błąd "Wystąpił błąd sprawdzania poprawności tokenu dostępu" podczas dołączania analizy pulpitu

Ten błąd jest zazwyczaj obserwowany po wygaśnięciu tokenu uwierzytelniania. Zazwyczaj odświeżanie strony odświeża token. Ten problem może jednak ustąpić, jeśli do konta używanego do analizy pulpitu na tablicy są stosowane jakieś zasady dostępu warunkowego. Dzienniki logowania usługi Azure AD możesz przejrzeć w portalu Azure Portal, aby sprawdzić, czy nie występują jakiekolwiek błędy logowania dla konta używanego do dołączania do usługi Desktop Analytics.

Aby uzyskać więcej informacji na temat dostępu warunkowego, odwiedź [stronę Planowanie wdrożenia dostępu warunkowego.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)
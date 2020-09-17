---
title: Wystąpił błąd podczas weryfikowania błędu tokenu dostępu podczas przeprowadzania na pokładzie funkcji analizy pulpitu
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783561"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Komunikat o błędzie "podczas sprawdzania poprawności tokenu dostępu" Wystąpił błąd podczas przechodzenia do funkcji analizy na komputerze

Ten błąd jest zwykle przestrzegany, gdy token uwierzytelniania wygasa. Zazwyczaj odświeżanie strony powoduje odświeżenie tokenu. Problem ten może jednak występować, jeśli w komputerze są zastosowane zasady dostępu warunkowego do konta używanego do analizy na płycie. Możesz przejrzeć dzienniki logowania do usługi Azure AD w portalu Azure, aby sprawdzić, czy konto używane do obsługi funkcji analizy komputerów jest dołączane do wszystkich niepowodzeń logowania.

Aby uzyskać więcej informacji na temat dostępu warunkowego, odwiedź witrynę [Planowanie wdrożenia dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).
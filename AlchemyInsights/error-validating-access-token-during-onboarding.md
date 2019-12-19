---
title: Wystąpił błąd podczas weryfikowania błąd tokenu dostępu podczas analizy pulpitu na pokład
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741238"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Błąd "Wystąpił błąd podczas sprawdzania poprawności tokenu dostępu" podczas dołączania Analytics pulpitu

Ten błąd jest zwykle obserwowane po wygaśnięciu tokenu uwierzytelniania. Zwykle odświeżanie strony odświeża token. Jednak ten problem może się powtarzać, jeśli istnieją jakiekolwiek zasady dostępu warunkowego stosowane do konta używanego do analizy pulpitu na pokładzie. Możesz przejrzeć dzienniki usługi Azure AD Sign in w witrynie Azure Portal, aby sprawdzić, czy są jakieś błędy logowania dla konta używanego do dołączania Analytics pulpitu.

Aby uzyskać więcej informacji na temat dostępu warunkowego, odwiedź stronę [Planowanie wdrożenia dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).
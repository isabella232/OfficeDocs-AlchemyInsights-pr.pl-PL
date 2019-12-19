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
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="132b8-102">Błąd "Wystąpił błąd podczas sprawdzania poprawności tokenu dostępu" podczas dołączania Analytics pulpitu</span><span class="sxs-lookup"><span data-stu-id="132b8-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="132b8-103">Ten błąd jest zwykle obserwowane po wygaśnięciu tokenu uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="132b8-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="132b8-104">Zwykle odświeżanie strony odświeża token.</span><span class="sxs-lookup"><span data-stu-id="132b8-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="132b8-105">Jednak ten problem może się powtarzać, jeśli istnieją jakiekolwiek zasady dostępu warunkowego stosowane do konta używanego do analizy pulpitu na pokładzie.</span><span class="sxs-lookup"><span data-stu-id="132b8-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="132b8-106">Możesz przejrzeć dzienniki usługi Azure AD Sign in w witrynie Azure Portal, aby sprawdzić, czy są jakieś błędy logowania dla konta używanego do dołączania Analytics pulpitu.</span><span class="sxs-lookup"><span data-stu-id="132b8-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="132b8-107">Aby uzyskać więcej informacji na temat dostępu warunkowego, odwiedź stronę [Planowanie wdrożenia dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="132b8-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>
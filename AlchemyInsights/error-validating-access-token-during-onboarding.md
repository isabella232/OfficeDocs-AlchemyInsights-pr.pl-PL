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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813698"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="b9713-102">Błąd "Wystąpił błąd sprawdzania poprawności tokenu dostępu" podczas dołączania analizy pulpitu</span><span class="sxs-lookup"><span data-stu-id="b9713-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="b9713-103">Ten błąd jest zazwyczaj obserwowany po wygaśnięciu tokenu uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="b9713-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="b9713-104">Zazwyczaj odświeżanie strony odświeża token.</span><span class="sxs-lookup"><span data-stu-id="b9713-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="b9713-105">Ten problem może jednak ustąpić, jeśli do konta używanego do analizy pulpitu na tablicy są stosowane jakieś zasady dostępu warunkowego.</span><span class="sxs-lookup"><span data-stu-id="b9713-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="b9713-106">Dzienniki logowania usługi Azure AD możesz przejrzeć w portalu Azure Portal, aby sprawdzić, czy nie występują jakiekolwiek błędy logowania dla konta używanego do dołączania do usługi Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="b9713-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="b9713-107">Aby uzyskać więcej informacji na temat dostępu warunkowego, odwiedź [stronę Planowanie wdrożenia dostępu warunkowego.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="b9713-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>
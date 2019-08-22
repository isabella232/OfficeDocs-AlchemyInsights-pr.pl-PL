---
title: Problemy z MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545185"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="5073f-102">Problemy z MFA</span><span class="sxs-lookup"><span data-stu-id="5073f-102">Issues with MFA</span></span>
<span data-ttu-id="5073f-103">Istnieje kilka rzeczy, które należy sprawdzić, czy użytkownicy nie mogą zalogować się za pomocą uwierzytelnianie wieloskładnikowe (MFA)</span><span class="sxs-lookup"><span data-stu-id="5073f-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="5073f-104">Danego użytkownika mogą być blokowane w portalu Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5073f-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="5073f-105">Jeśli tak się stanie, liczba prób uwierzytelniania do tego konkretnego użytkownika będą automatycznie odrzucane.</span><span class="sxs-lookup"><span data-stu-id="5073f-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="5073f-106">Wykonaj kroki opisane w tym artykule, aby odblokować je.</span><span class="sxs-lookup"><span data-stu-id="5073f-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="5073f-107">Jeśli odblokowanie użytkownika pomagało lub użytkownik nie jest zablokowany można spróbować zresetować MFA dla użytkownika i będą one ponownie przejść przez proces rejestrowania.</span><span class="sxs-lookup"><span data-stu-id="5073f-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="5073f-108">Wykonaj kroki opisane w tym artykule.</span><span class="sxs-lookup"><span data-stu-id="5073f-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="5073f-109">Jeśli jest po raz pierwszy MFA włączone i użytkownicy są w stanie zalogować się do klientów bez przeglądarek, takich jak Outlook, Skype itd, być może ADAL (uwierzytelnianie biblioteki usługi Active Directory) nie jest włączona na subskrypcję O365.</span><span class="sxs-lookup"><span data-stu-id="5073f-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="5073f-110">W tym przypadku trzeba będzie nawiązać PowerShell Online programu Exchange i uruchomienia tego apletu polecenia:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="5073f-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>
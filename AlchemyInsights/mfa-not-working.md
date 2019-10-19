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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545185"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="eca63-102">Problemy z MFA</span><span class="sxs-lookup"><span data-stu-id="eca63-102">Issues with MFA</span></span>
<span data-ttu-id="eca63-103">Istnieje kilka rzeczy, aby sprawdzić, czy użytkownicy nie mogą logować się przy użyciu uwierzytelniania wieloskładnikowego (MFA)</span><span class="sxs-lookup"><span data-stu-id="eca63-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="eca63-104">Usterce użytkownika mogą być blokowane w portalu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eca63-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="eca63-105">W takim przypadku uwierzytelnianie prób dla tego konkretnego użytkownika zostanie automatycznie odrzucone.</span><span class="sxs-lookup"><span data-stu-id="eca63-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="eca63-106">Wykonaj kroki opisane w tym artykule, aby je odblokować.</span><span class="sxs-lookup"><span data-stu-id="eca63-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="eca63-107">Jeśli Odblokowywanie użytkownika nie pomogło lub użytkownik nie jest zablokowany można spróbować zresetować MFA dla użytkownika i będą przechodzić przez proces rejestracji ponownie.</span><span class="sxs-lookup"><span data-stu-id="eca63-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="eca63-108">Należy postępować zgodnie z instrukcjami w tym artykule.</span><span class="sxs-lookup"><span data-stu-id="eca63-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="eca63-109">Jeśli jest to po raz pierwszy włączone uwierzytelnianie wieloskładnikowe i użytkownicy nie są w stanie zalogować się do klientów spoza przeglądarek, takich jak Outlook, Skype, itp., być może ADAL (Biblioteka uwierzytelniania usługi Active Directory) nie jest włączona w subskrypcji usługi 365.</span><span class="sxs-lookup"><span data-stu-id="eca63-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="eca63-110">W takim przypadku należy połączyć się z programu Exchange Online PowerShell i Uruchom to polecenie cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="eca63-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>
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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768847"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="04f5a-102">Problemy z usługą Azure MFA</span><span class="sxs-lookup"><span data-stu-id="04f5a-102">Issues with Azure MFA</span></span>
<span data-ttu-id="04f5a-103">Istnieje kilka rzeczy, aby sprawdzić, czy użytkownicy nie mogą zalogować się przy użyciu uwierzytelniania wieloskładnikowego (MFA)</span><span class="sxs-lookup"><span data-stu-id="04f5a-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="04f5a-104">Usterce użytkownika mogą być blokowane w portalu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="04f5a-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="04f5a-105">W takim przypadku uwierzytelnianie prób dla tego konkretnego użytkownika zostanie automatycznie odrzucone.</span><span class="sxs-lookup"><span data-stu-id="04f5a-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="04f5a-106">Wykonaj kroki opisane w tym artykule, aby je odblokować.</span><span class="sxs-lookup"><span data-stu-id="04f5a-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="04f5a-107">Jeśli Odblokowywanie użytkownika nie pomogło lub użytkownik nie jest zablokowany można spróbować zresetować MFA dla użytkownika i będą przechodzić przez proces rejestracji ponownie.</span><span class="sxs-lookup"><span data-stu-id="04f5a-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="04f5a-108">Należy postępować zgodnie z instrukcjami w tym artykule.</span><span class="sxs-lookup"><span data-stu-id="04f5a-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="04f5a-109">Jeśli jest to po raz pierwszy włączone uwierzytelnianie wieloskładnikowe i użytkownicy nie są w stanie zalogować się do klientów spoza przeglądarek, takich jak Outlook, Skype, itp., być może ADAL (Biblioteka uwierzytelniania usługi Active Directory) nie jest włączona w subskrypcji usługi 365.</span><span class="sxs-lookup"><span data-stu-id="04f5a-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="04f5a-110">W takim przypadku należy połączyć się z programu Exchange Online PowerShell i Uruchom to polecenie cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="04f5a-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>
---
title: Problemy z uwierzytelnianiem MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755141"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="5ce16-102">Problemy z usługą Azure MFA</span><span class="sxs-lookup"><span data-stu-id="5ce16-102">Issues with Azure MFA</span></span>
<span data-ttu-id="5ce16-103">Istnieje kilka sposobów sprawdzenia, czy użytkownicy nie mogą zalogować się przy użyciu uwierzytelniania wieloskładnikowego (MFA)</span><span class="sxs-lookup"><span data-stu-id="5ce16-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="5ce16-104">Użytkownik, którego dotyczy problem, może być zablokowany w portalu usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5ce16-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="5ce16-105">W takim przypadku próby uwierzytelnienia dla określonego użytkownika będą automatycznie odrzucane.</span><span class="sxs-lookup"><span data-stu-id="5ce16-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="5ce16-106">Wykonaj czynności opisane w tym artykule, aby odblokować je.</span><span class="sxs-lookup"><span data-stu-id="5ce16-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="5ce16-107">Jeśli odblokowanie użytkownika nie powiodło się lub użytkownik nie jest zablokowany, możesz spróbować zresetować uwierzytelnianie MFA dla użytkownika, a następnie ponownie przejść przez proces rejestracji.</span><span class="sxs-lookup"><span data-stu-id="5ce16-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="5ce16-108">Wykonaj czynności opisane w tym artykule.</span><span class="sxs-lookup"><span data-stu-id="5ce16-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="5ce16-109">Jeśli jest włączona funkcja MFA po raz pierwszy, a użytkownicy nie mogą logować się do klientów nieobsługujących przeglądarek, takich jak program Outlook, Skype itp., być może Biblioteka uwierzytelniania Active Directory jest niedostępna w ramach subskrypcji usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="5ce16-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="5ce16-110">W takim przypadku konieczne będzie nawiązanie połączenia z programem Exchange Online PowerShell i uruchomienie tego polecenia cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="5ce16-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>
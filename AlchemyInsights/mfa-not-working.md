---
title: Problemy z uwierzytelniania wieloskładnikowego
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810494"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="2f5c6-102">Problemy z uwierzytelniania wieloskładnikowego Azure</span><span class="sxs-lookup"><span data-stu-id="2f5c6-102">Issues with Azure MFA</span></span>
<span data-ttu-id="2f5c6-103">Jeśli użytkownicy nie mogą zalogować się przy użyciu uwierzytelniania wieloskładnikowego, należy sprawdzić kilka czynności.</span><span class="sxs-lookup"><span data-stu-id="2f5c6-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="2f5c6-104">Użytkownik, którego dotyczy problem, może zostać zablokowany w portalu usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2f5c6-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="2f5c6-105">W takim przypadku próby uwierzytelniania dla tego konkretnego użytkownika zostaną automatycznie odrzucone.</span><span class="sxs-lookup"><span data-stu-id="2f5c6-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="2f5c6-106">Wykonaj czynności opisane w tym artykule, aby je odblokować.</span><span class="sxs-lookup"><span data-stu-id="2f5c6-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="2f5c6-107">Jeśli odblokowanie użytkownika nie pomogło lub nie zostanie on zablokowany, możesz spróbować zresetować uwierzytelniania MFA dla użytkownika i ponownie przejść przez proces rejestracji.</span><span class="sxs-lookup"><span data-stu-id="2f5c6-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="2f5c6-108">Wykonaj czynności opisane w niniejszym artykule.</span><span class="sxs-lookup"><span data-stu-id="2f5c6-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="2f5c6-109">Jeśli po raz pierwszy włączono uwierzytelnianie MFA i użytkownicy nie mogą logować się do klientów innych niż przeglądarki, takich jak Outlook, Skype itp., być może biblioteka ADAL (Biblioteka uwierzytelniania usługi Active Directory) nie została włączona w Twojej subskrypcji usługi O365.</span><span class="sxs-lookup"><span data-stu-id="2f5c6-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="2f5c6-110">W takim przypadku musisz połączyć się z programem PowerShell dla usługi Exchange Online i uruchomić to polecenie cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="2f5c6-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>
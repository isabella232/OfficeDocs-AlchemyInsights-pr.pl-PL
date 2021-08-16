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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098612"
---
# <a name="issues-with-azure-mfa"></a>Problemy z uwierzytelniania wieloskładnikowego Azure
Jeśli użytkownicy nie mogą zalogować się przy użyciu uwierzytelniania wieloskładnikowego, należy sprawdzić kilka czynności.

1. Użytkownik, którego dotyczy problem, może być zablokowany w Azure Active Directory użytkowników. W takim przypadku próby uwierzytelniania dla tego konkretnego użytkownika zostaną automatycznie odrzucone. [Wykonaj czynności opisane w tym artykule, aby je odblokować.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jeśli odblokowanie użytkownika nie pomogło lub nie zostanie on zablokowany, możesz spróbować zresetować uwierzytelniania MFA dla użytkownika i ponownie przejść przez proces rejestracji. [Wykonaj czynności opisane w niniejszym artykule.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jeśli po raz pierwszy włączono uwierzytelnianie MFA i użytkownicy nie mogą logować się do klientów innych niż przeglądarki, takich jak Outlook, Skype itp., być może w Twojej subskrypcji usługi O365 nie włączono biblioteki ADAL (Active Directory Authentication Library). W takim przypadku musisz połączyć się z programem Exchange Online PowerShell i uruchomić to polecenie cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*
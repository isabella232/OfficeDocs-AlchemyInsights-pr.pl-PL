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
# <a name="issues-with-azure-mfa"></a>Problemy z uwierzytelniania wieloskładnikowego Azure
Jeśli użytkownicy nie mogą zalogować się przy użyciu uwierzytelniania wieloskładnikowego, należy sprawdzić kilka czynności.

1. Użytkownik, którego dotyczy problem, może zostać zablokowany w portalu usługi Azure Active Directory. W takim przypadku próby uwierzytelniania dla tego konkretnego użytkownika zostaną automatycznie odrzucone. [Wykonaj czynności opisane w tym artykule, aby je odblokować.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jeśli odblokowanie użytkownika nie pomogło lub nie zostanie on zablokowany, możesz spróbować zresetować uwierzytelniania MFA dla użytkownika i ponownie przejść przez proces rejestracji. [Wykonaj czynności opisane w niniejszym artykule.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jeśli po raz pierwszy włączono uwierzytelnianie MFA i użytkownicy nie mogą logować się do klientów innych niż przeglądarki, takich jak Outlook, Skype itp., być może biblioteka ADAL (Biblioteka uwierzytelniania usługi Active Directory) nie została włączona w Twojej subskrypcji usługi O365. W takim przypadku musisz połączyć się z programem PowerShell dla usługi Exchange Online i uruchomić to polecenie cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*
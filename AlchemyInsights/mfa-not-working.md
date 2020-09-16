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
# <a name="issues-with-azure-mfa"></a>Problemy z usługą Azure MFA
Istnieje kilka sposobów sprawdzenia, czy użytkownicy nie mogą zalogować się przy użyciu uwierzytelniania wieloskładnikowego (MFA)

1. Użytkownik, którego dotyczy problem, może być zablokowany w portalu usługi Azure Active Directory. W takim przypadku próby uwierzytelnienia dla określonego użytkownika będą automatycznie odrzucane. [Wykonaj czynności opisane w tym artykule, aby odblokować je.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jeśli odblokowanie użytkownika nie powiodło się lub użytkownik nie jest zablokowany, możesz spróbować zresetować uwierzytelnianie MFA dla użytkownika, a następnie ponownie przejść przez proces rejestracji. [Wykonaj czynności opisane w tym artykule.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jeśli jest włączona funkcja MFA po raz pierwszy, a użytkownicy nie mogą logować się do klientów nieobsługujących przeglądarek, takich jak program Outlook, Skype itp., być może Biblioteka uwierzytelniania Active Directory jest niedostępna w ramach subskrypcji usługi Office 365. W takim przypadku konieczne będzie nawiązanie połączenia z programem Exchange Online PowerShell i uruchomienie tego polecenia cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*
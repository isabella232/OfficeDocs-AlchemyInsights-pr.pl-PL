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
# <a name="issues-with-azure-mfa"></a>Problemy z usługą Azure MFA
Istnieje kilka rzeczy, aby sprawdzić, czy użytkownicy nie mogą zalogować się przy użyciu uwierzytelniania wieloskładnikowego (MFA)

1. Usterce użytkownika mogą być blokowane w portalu Azure Active Directory. W takim przypadku uwierzytelnianie prób dla tego konkretnego użytkownika zostanie automatycznie odrzucone. [Wykonaj kroki opisane w tym artykule, aby je odblokować.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jeśli Odblokowywanie użytkownika nie pomogło lub użytkownik nie jest zablokowany można spróbować zresetować MFA dla użytkownika i będą przechodzić przez proces rejestracji ponownie. [Należy postępować zgodnie z instrukcjami w tym artykule.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jeśli jest to po raz pierwszy włączone uwierzytelnianie wieloskładnikowe i użytkownicy nie są w stanie zalogować się do klientów spoza przeglądarek, takich jak Outlook, Skype, itp., być może ADAL (Biblioteka uwierzytelniania usługi Active Directory) nie jest włączona w subskrypcji usługi 365. W takim przypadku należy połączyć się z programu Exchange Online PowerShell i Uruchom to polecenie cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*
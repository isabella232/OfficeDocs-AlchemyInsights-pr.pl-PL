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
# <a name="issues-with-mfa"></a>Problemy z MFA
Istnieje kilka rzeczy, które należy sprawdzić, czy użytkownicy nie mogą zalogować się za pomocą uwierzytelnianie wieloskładnikowe (MFA)

1. Danego użytkownika mogą być blokowane w portalu Active Directory. Jeśli tak się stanie, liczba prób uwierzytelniania do tego konkretnego użytkownika będą automatycznie odrzucane. [Wykonaj kroki opisane w tym artykule, aby odblokować je.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jeśli odblokowanie użytkownika pomagało lub użytkownik nie jest zablokowany można spróbować zresetować MFA dla użytkownika i będą one ponownie przejść przez proces rejestrowania. [Wykonaj kroki opisane w tym artykule.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jeśli jest po raz pierwszy MFA włączone i użytkownicy są w stanie zalogować się do klientów bez przeglądarek, takich jak Outlook, Skype itd, być może ADAL (uwierzytelnianie biblioteki usługi Active Directory) nie jest włączona na subskrypcję O365. W tym przypadku trzeba będzie nawiązać PowerShell Online programu Exchange i uruchomienia tego apletu polecenia:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*
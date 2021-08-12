---
title: Wyszukiwanie i usuwanie wiadomości e-mail w organizacji
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948893"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Wyszukiwanie i usuwanie wiadomości e-mail w organizacji

Wykonaj następujące czynności:

1. Jeśli nie jesteś administratorem globalnym, aby wyszukiwać wiadomości, konto musi zostać dodane do grupy ról Menedżer **zbierania** elektronicznych materiałów dowodowych lub do roli zarządzania **wyszukiwaniem zgodności.** Aby usunąć wiadomości, musisz dołączyć  do grupy ról Zarządzanie organizacją lub do roli zarządzania wyszukiwaniem i **przeczyszczaniem.** Uprawnienia do tych ról są przypisywane w [Centrum & zgodności.](https://protection.office.com)
2. [Utwórz wyszukiwanie zawartości,](https://docs.microsoft.com/office365/securitycompliance/content-search) aby znaleźć wiadomość do usunięcia.
3. [Połączenie do programu PowerShell & w Centrum zgodności zabezpieczeń.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Jeśli korzystasz z uwierzytelniania wieloskładnikowego, zobacz następujące instrukcje: Połączenie do centrum zabezpieczeń & w programie PowerShell przy użyciu [uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Usunąć wiadomość: uruchom `New-ComplianceSearchAction` polecenie cmdlet, aby usunąć wiadomość. Usunięte wiadomości są przenoszone do folderu Elementy do odzyskania użytkownika. Aby uzyskać przykładowe polecenie, zobacz [Krok 3. Usunięcie wiadomości.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)

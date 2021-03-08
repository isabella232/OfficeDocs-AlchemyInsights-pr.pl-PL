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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525437"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Wyszukiwanie i usuwanie wiadomości e-mail w organizacji

Wykonaj następujące czynności:

1. Jeśli nie jesteś administratorem globalnym, aby można było wyszukiwać  wiadomości, konto musi zostać dodane do grupy ról Menedżer zbierania elektronicznych materiałów dowodowych lub do roli zarządzania **wyszukiwaniem zgodności.** Aby usunąć wiadomości, musisz dołączyć do grupy ról **Zarządzanie** organizacją lub do roli zarządzania wyszukiwaniem **i przeczyszczania.** Uprawnienia do tych ról są przypisywane w Centrum & [zgodności.](https://protection.office.com)
2. [Utwórz wyszukiwanie zawartości,](https://docs.microsoft.com/office365/securitycompliance/content-search) aby znaleźć wiadomość do usunięcia.
3. [Połącz się z programem PowerShell & w Centrum zabezpieczeń](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)i zgodności. Jeśli korzystasz z uwierzytelniania wieloskładnikowego, zobacz następujące instrukcje: Nawiązywanie połączenia z Centrum zabezpieczeń & Zgodności programu PowerShell przy użyciu uwierzytelniania [wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Usuń wiadomość: uruchom `New-ComplianceSearchAction` polecenie cmdlet, aby usunąć wiadomość. Usunięte wiadomości są przenoszone do folderu Elementy do odzyskania użytkownika. Aby uzyskać przykładowe polecenie, zobacz [Krok 3. Usunięcie wiadomości.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)

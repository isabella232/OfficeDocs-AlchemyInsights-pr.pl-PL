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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750012"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="0ff80-102">Wyszukiwanie i usuwanie wiadomości e-mail w organizacji</span><span class="sxs-lookup"><span data-stu-id="0ff80-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="0ff80-103">Wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="0ff80-103">Follow these steps:</span></span>

1. <span data-ttu-id="0ff80-104">Jeśli nie jesteś administratorem globalnym, aby wyszukiwać wiadomości, konto musi zostać dodane do grupy ról Menedżer **zbierania** elektronicznych materiałów dowodowych lub do roli zarządzania **wyszukiwaniem zgodności.**</span><span class="sxs-lookup"><span data-stu-id="0ff80-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="0ff80-105">Aby usunąć wiadomości, musisz dołączyć  do grupy ról Zarządzanie organizacją lub do roli zarządzania wyszukiwaniem i **przeczyszczaniem.**</span><span class="sxs-lookup"><span data-stu-id="0ff80-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="0ff80-106">Uprawnienia do tych ról są przypisywane w [Centrum & zgodności.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="0ff80-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="0ff80-107">[Utwórz wyszukiwanie zawartości,](https://docs.microsoft.com/office365/securitycompliance/content-search) aby znaleźć wiadomość do usunięcia.</span><span class="sxs-lookup"><span data-stu-id="0ff80-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="0ff80-108">[Połącz się z programem PowerShell & zabezpieczeń i zgodności.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0ff80-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="0ff80-109">Jeśli korzystasz z uwierzytelniania wieloskładnikowego, zobacz następujące instrukcje: Nawiązywanie połączenia z Centrum zgodności & [w programie PowerShell przy użyciu uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0ff80-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="0ff80-110">Usunąć wiadomość: uruchom `New-ComplianceSearchAction` polecenie cmdlet, aby usunąć wiadomość.</span><span class="sxs-lookup"><span data-stu-id="0ff80-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="0ff80-111">Usunięte wiadomości są przenoszone do folderu Elementy do odzyskania użytkownika.</span><span class="sxs-lookup"><span data-stu-id="0ff80-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="0ff80-112">Aby uzyskać przykładowe polecenie, zobacz [Krok 3. Usunięcie wiadomości.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="0ff80-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>

---
title: Szyfrowanie z wykorzystaniem reguł transportu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813878"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="2cec0-102">Szyfrowanie z wykorzystaniem reguł transportu</span><span class="sxs-lookup"><span data-stu-id="2cec0-102">Encryption with transport rules</span></span>

<span data-ttu-id="2cec0-103">W [centrum administracyjnym programu Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) możesz zastosować funkcję szyfrowania wiadomości pakietu Office w regułach przepływu poczty e-mail, aby wyzwalać szyfrowanie wiadomości.</span><span class="sxs-lookup"><span data-stu-id="2cec0-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="2cec0-104">Wybierz opcję **Zastosuj Szyfrowanie wiadomości usługi Office 365 i ochronę praw** w warunku Reguła transportu.</span><span class="sxs-lookup"><span data-stu-id="2cec0-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="2cec0-105">Aby uzyskać więcej informacji, zobacz [Definiowanie reguł przepływu poczty e-mail na potrzeby szyfrowania](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="2cec0-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="2cec0-106">W programie Powershell użyj polecenia cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) i ustaw parametr *ApplyOME* jako $true.</span><span class="sxs-lookup"><span data-stu-id="2cec0-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>

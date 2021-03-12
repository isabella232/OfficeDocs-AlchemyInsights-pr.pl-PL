---
title: Naprawianie zasad dzierżawy (zastępowanie akcji)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748993"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="7cb7d-102">Naprawianie zasad dzierżawy (zastępowanie akcji)</span><span class="sxs-lookup"><span data-stu-id="7cb7d-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="7cb7d-103">Ta wiadomość została podysłana przez zasady ochrony przed spamem w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="7cb7d-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="7cb7d-104">Aby przejrzeć zasady, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="7cb7d-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="7cb7d-105">Przejdź do Centrum zabezpieczeń [usługi Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143) zgodności , a następnie przejdź do strony Ochrona przed spamem przy zasadach zarządzania  >    >  [zagrożeniami.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="7cb7d-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="7cb7d-106">Sprawdź, czy  źródło zasad wskazuje następujące informacje: **Komunikat Add-Xheader/ModifySubject/Redirect/Delete/No action/ UDW**</span><span class="sxs-lookup"><span data-stu-id="7cb7d-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="7cb7d-107">Jeśli tak, na **karcie Niestandardowy** sprawdź ustawienia zasad, których dotyczyła wiadomość.</span><span class="sxs-lookup"><span data-stu-id="7cb7d-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="7cb7d-108">Możliwe, że wiadomość  wpłynęła na ustawienia standardowe zastosowane do wszystkich klientów usługi Exchange Online Protection.</span><span class="sxs-lookup"><span data-stu-id="7cb7d-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="7cb7d-109">Aby uzyskać więcej informacji na temat konfigurowania zasad filtrowania spamu, zobacz [Konfigurowanie zasad filtru spamu.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="7cb7d-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>

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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695698"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="8dbc7-102">Naprawianie zasad dzierżawy (zastępowanie akcji)</span><span class="sxs-lookup"><span data-stu-id="8dbc7-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="8dbc7-103">Ta wiadomość ma wpływ na zasady ochrony przed spamem w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="8dbc7-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="8dbc7-104">Aby przejrzeć zasady, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="8dbc7-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="8dbc7-105">Przejdź do Centrum zabezpieczeń usługi [Office 365 & zgodności,](https://go.microsoft.com/fwlink/p/?linkid=2077143)a następnie przejdź do strony Ochrona przed spamem w zasadach zarządzania   >    >  [zagrożeniami.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="8dbc7-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="8dbc7-106">Sprawdź, czy  źródło zasad wskazuje następujące informacje: **Add-Xheader/ModifySubject/Redirect/Delete/No action/BCC message**</span><span class="sxs-lookup"><span data-stu-id="8dbc7-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="8dbc7-107">Jeśli tak, na karcie **Niestandardowe** sprawdź ustawienia zasad, które wpłynęły na wiadomość.</span><span class="sxs-lookup"><span data-stu-id="8dbc7-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="8dbc7-108">Możliwe, że wiadomość  wpłynęła na ustawienia standardowe zastosowane do wszystkich klientów usługi Exchange Online Protection.</span><span class="sxs-lookup"><span data-stu-id="8dbc7-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="8dbc7-109">Aby uzyskać więcej informacji na temat konfigurowania zasad filtrowania spamu, zobacz [Konfigurowanie zasad filtrowania spamu.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="8dbc7-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>

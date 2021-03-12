---
title: Naprawianie reguł transportu
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750579"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="de9cd-102">Naprawianie reguł transportu</span><span class="sxs-lookup"><span data-stu-id="de9cd-102">Fix transport rules</span></span>

<span data-ttu-id="de9cd-103">Ta wiadomość została wpłynęła na niestandardową regułę przepływu poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="de9cd-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="de9cd-104">Aby sprawdzić dokładną regułę, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="de9cd-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="de9cd-105">W wynikach przesyłania w **obszarze Informacje dodatkowe** zanotuj identyfikator **GUID** lub **nazwę zasad.**</span><span class="sxs-lookup"><span data-stu-id="de9cd-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="de9cd-106">Uruchom powłokę zarządzania programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="de9cd-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="de9cd-107">Aby uzyskać więcej informacji, [zobacz Otwieranie powłoki zarządzania programu Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="de9cd-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="de9cd-108">Uruchom to polecenie (przy użyciu identyfikatora GUID z Twojego przesłania):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="de9cd-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="de9cd-109">Przejrzyj opis, aby zobaczyć skonfigurowane warunki, które wpłynęły na wiadomość.</span><span class="sxs-lookup"><span data-stu-id="de9cd-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="de9cd-110">Aby dowiedzieć się więcej, [zobacz Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="de9cd-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>

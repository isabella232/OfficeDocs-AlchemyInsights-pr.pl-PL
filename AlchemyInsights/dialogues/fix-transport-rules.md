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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695857"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="27048-102">Naprawianie reguł transportu</span><span class="sxs-lookup"><span data-stu-id="27048-102">Fix transport rules</span></span>

<span data-ttu-id="27048-103">Wiadomość wpłynęła na niestandardową regułę przepływu poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="27048-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="27048-104">Aby zapoznać się z dokładną regułą, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="27048-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="27048-105">W wynikach przesyłania w obszarze **Informacje dodatkowe** zwróć uwagę na identyfikator **GUID** lub **nazwę zasad.**</span><span class="sxs-lookup"><span data-stu-id="27048-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="27048-106">Uruchom powłokę zarządzania programem Exchange.</span><span class="sxs-lookup"><span data-stu-id="27048-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="27048-107">Aby uzyskać więcej informacji, [zobacz Otwieranie powłoki zarządzania programem Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="27048-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="27048-108">Uruchom to polecenie (używając identyfikatora GUID z Twojego przesłania):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="27048-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="27048-109">Przejrzyj opis, aby zobaczyć skonfigurowane warunki, które wpłynęły na wiadomość.</span><span class="sxs-lookup"><span data-stu-id="27048-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="27048-110">Aby dowiedzieć się więcej, [zobacz Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="27048-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>

---
title: Włączanie domeny niestandardowej dla funkcji DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749206"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="a4e3a-102">Włączanie domeny niestandardowej dla funkcji DKIM</span><span class="sxs-lookup"><span data-stu-id="a4e3a-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="a4e3a-103">Po utworzeniu rekordów CNAME dla domen niestandardowych należy włączyć tę domenę.</span><span class="sxs-lookup"><span data-stu-id="a4e3a-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="a4e3a-104">Aby włączyć domenę, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="a4e3a-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="a4e3a-105">Przejdź do Centrum [administracyjnego programu Exchange.](https://outlook.office365.com/ecp/)</span><span class="sxs-lookup"><span data-stu-id="a4e3a-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="a4e3a-106">W okienku po lewej stronie wybierz **pozycję ochrona > dkim**.</span><span class="sxs-lookup"><span data-stu-id="a4e3a-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="a4e3a-107">Wybierz domenę, a następnie w obszarze Podpisz wiadomości dla tej domeny za pomocą podpisów **DKIM** kliknij pozycję **Włącz**.</span><span class="sxs-lookup"><span data-stu-id="a4e3a-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="a4e3a-108">Powtórz ten krok dla każdej domeny.</span><span class="sxs-lookup"><span data-stu-id="a4e3a-108">Repeat this step for each domain.</span></span>


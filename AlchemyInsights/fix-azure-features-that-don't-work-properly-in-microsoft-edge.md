---
title: Co zrobić, jeśli funkcje platformy Azure nie działają poprawnie w programie Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583787"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="fc91d-102">Co zrobić, jeśli funkcje platformy Azure nie działają poprawnie w programie Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="fc91d-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="fc91d-103">W programie Microsoft Edge występują [znane problemy](https://go.microsoft.com/fwlink/?linkid=2140608) dotyczące stref zabezpieczeń, które mogą wpływać na sposób logowania użytkowników platformy Azure do centrum administracyjnego systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="fc91d-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="fc91d-104">Jeśli masz problemy z korzystaniem z funkcji platformy Azure w programie Microsoft Edge, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="fc91d-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="fc91d-105">W menu **Start** Wyszukaj polecenie **Opcje internetowe** i wybierz je.</span><span class="sxs-lookup"><span data-stu-id="fc91d-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="fc91d-106">W oknie dialogowym **Właściwości internetowe** przejdź do karty **zabezpieczenia** .</span><span class="sxs-lookup"><span data-stu-id="fc91d-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="fc91d-107">Wybierz strefę **Zaufane witryny** , a następnie wybierz przycisk **witryny** .</span><span class="sxs-lookup"><span data-stu-id="fc91d-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="fc91d-108">W oknie dialogowym **Zaufane witryny** Dodaj adres URL bramy oraz [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) pozycję, a następnie wybierz pozycję **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="fc91d-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="fc91d-109">W oknie dialogowym **Właściwości internetowe** przejdź do karty **prywatność** .</span><span class="sxs-lookup"><span data-stu-id="fc91d-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="fc91d-110">W sekcji **Blokowanie wyskakiwania okien** wybierz pozycję **Ustawienia**.</span><span class="sxs-lookup"><span data-stu-id="fc91d-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="fc91d-111">W otwartym oknie dialogowym Dodaj adres URL bramy oraz [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) pozycję, a następnie wybierz pozycję **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="fc91d-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>

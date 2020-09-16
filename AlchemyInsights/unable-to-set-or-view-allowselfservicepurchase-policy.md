---
title: Nie można ustawić lub wyświetlić zasad AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735209"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="e1ba1-102">Nie można ustawić lub wyświetlić zasad AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="e1ba1-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="e1ba1-103">Podczas próby ustawienia lub wyświetlenia zasad AllowSelfServicePurchase jest wyświetlany następujący komunikat o błędzie:</span><span class="sxs-lookup"><span data-stu-id="e1ba1-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="e1ba1-104">*HandleError: nie można pobrać zasad dotyczących produktu z PolicyId "AllowSelfServicePurchase", ErrorMessage — połączenie podstawowe zostało zakończone: Wystąpił nieoczekiwany błąd podczas wysyłania.*</span><span class="sxs-lookup"><span data-stu-id="e1ba1-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="e1ba1-105">Może to być spowodowane starszą wersją protokołu TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="e1ba1-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="e1ba1-106">Aby połączyć usługę MSCommerce, musisz użyć protokołu TLS 1,2 lub nowszego.</span><span class="sxs-lookup"><span data-stu-id="e1ba1-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="e1ba1-107">Spróbuj wykonać poniższe czynności, aby włączyć/ustawić protokół TLS na 1,2, sprawdź, a następnie ponów próbę.</span><span class="sxs-lookup"><span data-stu-id="e1ba1-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="e1ba1-108">W wierszu polecenia programu PowerShell (PS C: \) wprowadź następujące polecenie, aby ustawić protokół TLS w wersji 1,2:</span><span class="sxs-lookup"><span data-stu-id="e1ba1-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="e1ba1-109">Sprawdź używane protokoły TLS za pomocą następującego polecenia:</span><span class="sxs-lookup"><span data-stu-id="e1ba1-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="e1ba1-110">Spróbuj ponownie wykonać polecenia Pobierz lub Aktualizuj stosownie do potrzeb.</span><span class="sxs-lookup"><span data-stu-id="e1ba1-110">Retry the Get or Update commands as needed.</span></span>


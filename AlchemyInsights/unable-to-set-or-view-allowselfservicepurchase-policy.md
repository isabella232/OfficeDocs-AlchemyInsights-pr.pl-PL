---
title: Nie można ustawić ani wyświetlić zasad AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826101"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="01c90-102">Nie można ustawić ani wyświetlić zasad AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="01c90-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="01c90-103">Podczas próby ustawienia lub wyświetlenia zasad AllowSelfServicePurchase jest wyświetlany następujący komunikat o błędzie:</span><span class="sxs-lookup"><span data-stu-id="01c90-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="01c90-104">*HandleError: Nie można pobrać zasad produktu przy użyciu wartości PolicyId 'AllowSelfServicePurchase', ErrorMessage — połączenie źródłowe zostało zamknięte: Wystąpił nieoczekiwany błąd podczas wysyłania.*</span><span class="sxs-lookup"><span data-stu-id="01c90-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="01c90-105">Może to być spowodowane starszą wersją usługi Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="01c90-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="01c90-106">Aby połączyć usługę MS Commerce, musisz użyć usługi TLS 1.2 lub większej.</span><span class="sxs-lookup"><span data-stu-id="01c90-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="01c90-107">Spróbuj wykonać poniższe czynności, aby włączyć/ustawić dla protokołu TLS wartość 1.2, zweryfikować i ponowić próbę.</span><span class="sxs-lookup"><span data-stu-id="01c90-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="01c90-108">W wierszu polecenia programu PowerShell (PS C: wprowadź następujące polecenie, aby ustawić protokół \) TLS na wersję 1.2:</span><span class="sxs-lookup"><span data-stu-id="01c90-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="01c90-109">Sprawdź, czy są używani protokoły TLS, za pomocą następującego polecenia:</span><span class="sxs-lookup"><span data-stu-id="01c90-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="01c90-110">W razie potrzeby ponownie spróbuj wykonać polecenia Pobierz lub Aktualizuj.</span><span class="sxs-lookup"><span data-stu-id="01c90-110">Retry the Get or Update commands as needed.</span></span>


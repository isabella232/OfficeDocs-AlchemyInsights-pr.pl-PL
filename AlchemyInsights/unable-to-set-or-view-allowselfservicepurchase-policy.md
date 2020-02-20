---
title: Nie można ustawić lub wyświetlić zasad Zezwalania na zakup usługi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158571"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="f8f3c-102">Nie można ustawić lub wyświetlić zasad Zezwalania na zakup usługi</span><span class="sxs-lookup"><span data-stu-id="f8f3c-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="f8f3c-103">Podczas próby ustawienia lub wyświetlenia zasad Zezwalania na zakup usługi wyświetlany jest następujący komunikat o błędzie:</span><span class="sxs-lookup"><span data-stu-id="f8f3c-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="f8f3c-104">*HandleError: Nie można pobrać zasady produktu z PolicyId "AllowSelfServicePurchase", ErrorMessage — połączenie źródłowe zostało zamknięte: Wystąpił nieoczekiwany błąd podczas wysyłania.*</span><span class="sxs-lookup"><span data-stu-id="f8f3c-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="f8f3c-105">Może to być spowodowane starszą wersją zabezpieczeń warstwy transportowej (TLS).</span><span class="sxs-lookup"><span data-stu-id="f8f3c-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="f8f3c-106">Aby połączyć usługę MSCommerce, musisz użyć tls 1.2 lub więcej.</span><span class="sxs-lookup"><span data-stu-id="f8f3c-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="f8f3c-107">Spróbuj wykonać następujące kroki, aby włączyć/ustawić protokół TLS na 1.2, zweryfikować i ponowić próbę.</span><span class="sxs-lookup"><span data-stu-id="f8f3c-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="f8f3c-108">W wierszu polecenia programu PowerShell (PS C:\) wprowadź następujące polecenie, aby ustawić protokół TLS na wersję 1.2:</span><span class="sxs-lookup"><span data-stu-id="f8f3c-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="f8f3c-109">Sprawdź używane protokoły TLS za pomocą następującego polecenia:</span><span class="sxs-lookup"><span data-stu-id="f8f3c-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="f8f3c-110">W razie potrzeby ponów próbę polecenia Pobierz lub Aktualizuj.</span><span class="sxs-lookup"><span data-stu-id="f8f3c-110">Retry the Get or Update commands as needed.</span></span>


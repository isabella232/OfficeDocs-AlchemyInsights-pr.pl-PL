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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091742"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="07ccd-102">Nie można ustawić lub wyświetlić zasad Zezwalania na zakup usługi</span><span class="sxs-lookup"><span data-stu-id="07ccd-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="07ccd-103">Podczas próby ustawienia lub wyświetlenia zasad Zezwalania na zakup usługi wyświetlany jest następujący komunikat o błędzie:</span><span class="sxs-lookup"><span data-stu-id="07ccd-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="07ccd-104">*HandleError: Nie można pobrać zasady produktu z PolicyId "AllowSelfServicePurchase", ErrorMessage — połączenie źródłowe zostało zamknięte: Wystąpił nieoczekiwany błąd podczas wysyłania.*</span><span class="sxs-lookup"><span data-stu-id="07ccd-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="07ccd-105">Może to być spowodowane starszą wersją zabezpieczeń warstwy transportowej (TLS).</span><span class="sxs-lookup"><span data-stu-id="07ccd-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="07ccd-106">Aby połączyć usługę MSCommerce, musisz użyć tls 1.2 lub więcej.</span><span class="sxs-lookup"><span data-stu-id="07ccd-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="07ccd-107">Spróbuj wykonać następujące kroki, aby włączyć/ustawić protokół TLS na 1.2, zweryfikować i ponowić próbę.</span><span class="sxs-lookup"><span data-stu-id="07ccd-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="07ccd-108">W wierszu polecenia programu PowerShell (PS C:\) wprowadź następujące polecenie, aby ustawić protokół TLS na wersję 1.2:</span><span class="sxs-lookup"><span data-stu-id="07ccd-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="07ccd-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="07ccd-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="07ccd-110">Sprawdź używane protokoły TLS za pomocą następującego polecenia:</span><span class="sxs-lookup"><span data-stu-id="07ccd-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="07ccd-111">\[Net.ServicePointManager]::SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="07ccd-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="07ccd-112">W razie potrzeby ponów próbę polecenia Pobierz lub Aktualizuj.</span><span class="sxs-lookup"><span data-stu-id="07ccd-112">Retry the Get or Update commands as needed.</span></span>


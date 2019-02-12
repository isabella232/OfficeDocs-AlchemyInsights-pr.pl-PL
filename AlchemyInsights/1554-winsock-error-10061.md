---
title: Błąd warstwy Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903116"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="f2c0e-102">Błąd warstwy Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="f2c0e-102">Winsock error 10061</span></span>

<span data-ttu-id="f2c0e-p101">Ten kod błędu oznacza, że usługi Office 365, nie można ustanowić gniazda TCP (połączenie) z hosta docelowego. Najbardziej prawdopodobną przyczyną tego błędu jest problem z konfiguracją zapory. Aby rozwiązać ten problem, sprawdź następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="f2c0e-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="f2c0e-106">Sprawdź konfigurację zapory przy użyciu informacji z [zakresów adresów IP i adresy URL usługi Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="f2c0e-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="f2c0e-107">Jeśli błąd jest specyficzny na Exchange Online ochrony (podniesienie uprawnień), możesz powinny zostały wcześniej zgłoszone do zmiany na [adresy IP ochrony Online programu Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="f2c0e-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="f2c0e-108">Sprawdź, czy usługodawcy internetowego (ISP) nie blokuje port.</span><span class="sxs-lookup"><span data-stu-id="f2c0e-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="f2c0e-109">Sprawdź inteligentne ustawienia serwera hosta i docelowego w złącza.</span><span class="sxs-lookup"><span data-stu-id="f2c0e-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="f2c0e-110">Należy zauważyć, że usługi Office 365 nie blokuje połączenia *przychodzące* w ten sposób.</span><span class="sxs-lookup"><span data-stu-id="f2c0e-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  


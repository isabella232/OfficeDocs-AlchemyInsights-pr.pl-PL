---
title: 1554 Błąd Winsocka 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766179"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="0df2f-102">Błąd Winsocka 10061</span><span class="sxs-lookup"><span data-stu-id="0df2f-102">Winsock error 10061</span></span>

<span data-ttu-id="0df2f-103">Ten kod błędu oznacza, że firma Microsoft nie może ustanowić gniazda TCP (połączenia) z hostem docelowym.</span><span class="sxs-lookup"><span data-stu-id="0df2f-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="0df2f-104">Najbardziej prawdopodobną przyczyną tego błędu jest problem z konfiguracją zapory.</span><span class="sxs-lookup"><span data-stu-id="0df2f-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="0df2f-105">Aby rozwiązać ten problem, sprawdź następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="0df2f-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="0df2f-106">Weryfikowanie konfiguracji zapory za pomocą informacji w [adresach URL i zakresach adresów IP usługi Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="0df2f-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="0df2f-107">Jeśli błąd dotyczy programu Exchange Online Protection (EOP), użytkownik powinien zostać wcześniej powiadomiony o zmianie [adresów IP ochrony usługi Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)Protection .</span><span class="sxs-lookup"><span data-stu-id="0df2f-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="0df2f-108">Sprawdź, czy usługodawca internetowy nie blokuje portu.</span><span class="sxs-lookup"><span data-stu-id="0df2f-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="0df2f-109">Sprawdź ustawienia hosta inteligentnego i serwera docelowego w łącznikach.</span><span class="sxs-lookup"><span data-stu-id="0df2f-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="0df2f-110">Należy zauważyć, że usługa Microsoft 365 nie blokuje połączeń *przychodzących* w ten sposób.</span><span class="sxs-lookup"><span data-stu-id="0df2f-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>

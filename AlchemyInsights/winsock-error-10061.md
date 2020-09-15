---
title: 1554 błąd Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698872"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="de923-102">Błąd Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="de923-102">Winsock error 10061</span></span>

<span data-ttu-id="de923-103">Ten kod błędu oznacza, że firma Microsoft nie mogła ustanowić gniazda TCP (połączenia) z hostem docelowym.</span><span class="sxs-lookup"><span data-stu-id="de923-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="de923-104">Najbardziej prawdopodobną przyczyną tego błędu jest problem z konfiguracją zapory.</span><span class="sxs-lookup"><span data-stu-id="de923-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="de923-105">Aby rozwiązać ten problem, sprawdź następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="de923-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="de923-106">Weryfikowanie konfiguracji zapory przy użyciu informacji z [adresów URL i zakresów adresów IP programu Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="de923-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="de923-107">Jeśli błąd jest specyficzny dla usługi Exchange Online Protection (EOP), należy wcześniej powiadomić o zmianach [adresów IP usługi Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="de923-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="de923-108">Sprawdź, czy Twój dostawca usług internetowych (ISP) nie blokuje portu.</span><span class="sxs-lookup"><span data-stu-id="de923-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="de923-109">Sprawdź ustawienia hosta inteligentnego i serwera docelowego w łącznikach.</span><span class="sxs-lookup"><span data-stu-id="de923-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="de923-110">Pamiętaj, że program Microsoft 365 nie blokuje połączeń *przychodzących* w ten sposób.</span><span class="sxs-lookup"><span data-stu-id="de923-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>

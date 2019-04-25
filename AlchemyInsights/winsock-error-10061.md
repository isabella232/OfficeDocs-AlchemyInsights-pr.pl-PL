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
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419990"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="0fde0-102">Błąd warstwy Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="0fde0-102">Winsock error 10061</span></span>

<span data-ttu-id="0fde0-103">Ten kod błędu oznacza, że usługi Office 365, nie można ustanowić gniazda TCP (połączenie) z hosta docelowego.</span><span class="sxs-lookup"><span data-stu-id="0fde0-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="0fde0-104">Najbardziej prawdopodobną przyczyną tego błędu jest problem z konfiguracją zapory.</span><span class="sxs-lookup"><span data-stu-id="0fde0-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="0fde0-105">Aby rozwiązać ten problem, sprawdź następujące ustawienia:</span><span class="sxs-lookup"><span data-stu-id="0fde0-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="0fde0-106">Sprawdź konfigurację zapory przy użyciu informacji z [zakresów adresów IP i adresy URL usługi Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="0fde0-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="0fde0-107">Jeśli błąd jest specyficzny na Exchange Online ochrony (podniesienie uprawnień), możesz powinny zostały wcześniej zgłoszone do zmiany na [adresy IP ochrony Online programu Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0fde0-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="0fde0-108">Sprawdź, czy usługodawcy internetowego (ISP) nie blokuje port.</span><span class="sxs-lookup"><span data-stu-id="0fde0-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="0fde0-109">Sprawdź inteligentne ustawienia serwera hosta i docelowego w złącza.</span><span class="sxs-lookup"><span data-stu-id="0fde0-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="0fde0-110">Należy zauważyć, że usługi Office 365 nie blokuje połączenia *przychodzące* w ten sposób.</span><span class="sxs-lookup"><span data-stu-id="0fde0-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>

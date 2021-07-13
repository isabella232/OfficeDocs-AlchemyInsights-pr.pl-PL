---
title: Pula przekazywania połączeń wychodzących
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381857"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="52ff6-102">Pula przekazywania połączeń wychodzących</span><span class="sxs-lookup"><span data-stu-id="52ff6-102">Outbound relay pool</span></span>

<span data-ttu-id="52ff6-103">Firma Microsoft wprowadza pewne zmiany w konfiguracji przekazywania lub przesyłania dalej poczty e-mail za pośrednictwem Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="52ff6-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="52ff6-104">Wiadomości w określonych scenariuszach są przekazywane dalej lub przekazywane przez Microsoft 365 przy użyciu specjalnej puli przekazywania.</span><span class="sxs-lookup"><span data-stu-id="52ff6-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="52ff6-105">Wiadomości wysłane przy użyciu puli przekazywania mogą trafiać do folderu wiadomości-śmieci adresata.</span><span class="sxs-lookup"><span data-stu-id="52ff6-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="52ff6-106">Aby uzyskać więcej informacji, zobacz [Pule dostarczania połączeń wychodzących](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="52ff6-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="52ff6-107">Aby uniknąć sytuacji używającej puli przekazywania, upewnij się, że wiadomości przekazane/przekazane spełniają jedno z następujących kryteriów:</span><span class="sxs-lookup"><span data-stu-id="52ff6-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="52ff6-108">Nadawca ruchu wychodzącego jest zaakceptowaną domeną dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="52ff6-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="52ff6-109">Spf (Sender Policy Framework) przechodzi, gdy przychodzi wiadomość do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="52ff6-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="52ff6-110">DKIM (DomainKeys Identified Mail) w domenie nadawcy P2 przechodzi, gdy przychodzi wiadomość do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="52ff6-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="52ff6-111">Wiadomości spełniające powyższe kryteria nie są przekazywane przez pulę przekazywania.</span><span class="sxs-lookup"><span data-stu-id="52ff6-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="52ff6-112">Jeśli rekord MX domeny wskazuje serwer innej firmy lub serwer lokalne, użyj funkcji rozszerzonego filtrowania, aby upewnić się, że weryfikacja SPF jest prawidłowa dla przychodzącej poczty e-mail i aby uniknąć wysyłania wiadomości e-mail za pośrednictwem puli przekazywania.</span><span class="sxs-lookup"><span data-stu-id="52ff6-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="52ff6-113">**Jak możemy stwierdzić, czy na nas wpływa pula przekazywania?**</span><span class="sxs-lookup"><span data-stu-id="52ff6-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="52ff6-114">Jeśli w przesyłanych lub przesyłanych wiadomościach e-mail jest stosowane jedno z powyższych kryteriów, wiadomości nie będą przekazywane przez pulę przekazywania.</span><span class="sxs-lookup"><span data-stu-id="52ff6-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="52ff6-115">Jeśli jednak wiadomość jest wysyłana za pośrednictwem puli przekazywania, adres IP serwera ruchu wychodzącego należy do zakresu 40.95.0.0/16, a nazwa serwera ruchu wychodzącego zawiera nazwę **rly.**</span><span class="sxs-lookup"><span data-stu-id="52ff6-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>


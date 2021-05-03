---
title: Jakość udostępniania ekranu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/26/2021
ms.locfileid: "52125441"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="a7757-102">Jakość udostępniania ekranu</span><span class="sxs-lookup"><span data-stu-id="a7757-102">Screen sharing quality</span></span>

<span data-ttu-id="a7757-103">W większości przypadków problemy z jakością związane z udostępnianiem ekranu mają ograniczoną przepustowość po stronie klienta.</span><span class="sxs-lookup"><span data-stu-id="a7757-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="a7757-104">Tam, gdzie przepustowość nie jest ograniczona, program Teams optymalizuje jakość multimediów, w tym rozdzielczość wideo 1080p, do 30 pikseli na obraz wideo, 15fps dla zawartości i dźwięk o wysokiej wierności.</span><span class="sxs-lookup"><span data-stu-id="a7757-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="a7757-105">Teams poziom użycia przepustowości jest zawsze podyskuszowy i może dostarczać obraz o jakości HD w przepustowości poniżej 1,2 Mb/s.</span><span class="sxs-lookup"><span data-stu-id="a7757-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="a7757-106">Rzeczywiste wykorzystanie przepustowości w poszczególnych połączeniach audio/wideo lub spotkaniach zależy od czynników, takich jak układ wideo, rozdzielczość wideo i liczba klatek wideo na sekundę.</span><span class="sxs-lookup"><span data-stu-id="a7757-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="a7757-107">Gdy dostępna jest większa przepustowość, jakość i użycie rosną, aby zapewnić najlepsze środowisko.</span><span class="sxs-lookup"><span data-stu-id="a7757-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="a7757-108">W poniższej tabeli opisano Teams przepustowości:</span><span class="sxs-lookup"><span data-stu-id="a7757-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="a7757-109">**Scenariusze przepustowości (w górę/w dół)**</span><span class="sxs-lookup"><span data-stu-id="a7757-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="a7757-110">Równorzędne połączenia audio 30 kb/s</span><span class="sxs-lookup"><span data-stu-id="a7757-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="a7757-111">Równorzędne połączenia audio i udostępnianie ekranu o rozdzielczości 130 kb/s</span><span class="sxs-lookup"><span data-stu-id="a7757-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="a7757-112">500 kb/s — połączenia wideo o jakości peer-to-peer 360p przy 30fps</span><span class="sxs-lookup"><span data-stu-id="a7757-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="a7757-113">1,2 Mb/s Peer-to-peer HD video calling with resolution of HD 720p at 30fps</span><span class="sxs-lookup"><span data-stu-id="a7757-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="a7757-114">1,5 Mb/s Peer-to-peer HD video calling with resolution of HD 1080p at 30fps</span><span class="sxs-lookup"><span data-stu-id="a7757-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="a7757-115">Grupowe rozmowy wideo o jakości 500 kb/s/s</span><span class="sxs-lookup"><span data-stu-id="a7757-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="a7757-116">Grupowe rozmowy wideo w jakości HD 1 Mb/s (klipy wideo 540p na ekranie 1080p)</span><span class="sxs-lookup"><span data-stu-id="a7757-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="a7757-117">Aby uzyskać więcej informacji, [zobacz Przygotowanie sieci organizacji](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements) na Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a7757-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>
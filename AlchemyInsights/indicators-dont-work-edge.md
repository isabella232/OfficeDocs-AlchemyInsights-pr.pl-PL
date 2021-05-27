---
title: Wskaźniki nie działają przy użyciu przeglądarki Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676462"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="27143-102">Wskaźniki nie działają przy użyciu przeglądarki Edge</span><span class="sxs-lookup"><span data-stu-id="27143-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="27143-103">Po utworzeniu wskaźnika nie jest on ujmowany w edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="27143-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="27143-104">Aby uzyskać więcej informacji, zobacz Tworzenie wskaźników adresów [IP oraz adresów URL/domen.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="27143-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="27143-105">Krok 1. Upewnij się, że są</span><span class="sxs-lookup"><span data-stu-id="27143-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="27143-106">Sprawdź, czy wskaźnik jest poprawny (nie literówki w adresie IP/adresie URL, prawidłowa akcja, właściwe grupy RBAC).</span><span class="sxs-lookup"><span data-stu-id="27143-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="27143-107">Poczekaj co najmniej 2 godziny po utworzeniu wskaźnika, aby uwzględnić wszelkie możliwe opóźnienia.</span><span class="sxs-lookup"><span data-stu-id="27143-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="27143-108">Upewnij się, że system(-y) jest wnoszony do programu Microsoft Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="27143-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="27143-109">Sprawdź, czy system(y) może komunikować się z chmurą.</span><span class="sxs-lookup"><span data-stu-id="27143-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="27143-110">Sprawdź, czy filtr Smartscreen jest włączony i osiągalny, przechodząc do [witryny testowej.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="27143-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="27143-111">Krok 2. Rozwiązywanie potencjalnego problemu</span><span class="sxs-lookup"><span data-stu-id="27143-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="27143-112">Upewnij się, że klient spełnia wymagania.</span><span class="sxs-lookup"><span data-stu-id="27143-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="27143-113">Aby uzyskać szczegółowe informacje, [zobacz Tworzenie wskaźników adresów IP oraz adresów URL/domen.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="27143-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="27143-114">Upewnij się, że używasz najnowszej wersji przeglądarki Edge.</span><span class="sxs-lookup"><span data-stu-id="27143-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="27143-115">Aby dowiedzieć się, która wersja jest najnowsza, zobacz Dowiedz się, [Microsoft Edge masz.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="27143-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="27143-116">Uruchom ponownie przeglądarkę Edge.</span><span class="sxs-lookup"><span data-stu-id="27143-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="27143-117">Przejdź do witryny, dla której masz wskaźnik konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="27143-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="27143-118">Jeśli witryna nie jest wyświetlana zgodnie z oczekiwaniami, przejdź do kroku 3.</span><span class="sxs-lookup"><span data-stu-id="27143-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="27143-119">Krok 3. Zbieranie danych</span><span class="sxs-lookup"><span data-stu-id="27143-119">Step 3: Collect data</span></span>

- <span data-ttu-id="27143-120">Zbierz **dane diagnostyczne MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="27143-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="27143-121">Aby uzyskać instrukcje, [zobacz Problemy z komputerami dołączania do programu Microsoft Defender dla punktu końcowego.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="27143-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="27143-122">Jeśli wiesz, jak instalować i zbierać dane śledzenia fiddlera, zobacz [Telerik Fiddler.](http://www.telerik.com/fiddler)</span><span class="sxs-lookup"><span data-stu-id="27143-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="27143-123">Jeśli wolisz wskazówki z pomocy technicznej firmy Microsoft, wybierz ikonę Pomoc techniczna poniżej, aby otworzyć sprawę pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="27143-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>

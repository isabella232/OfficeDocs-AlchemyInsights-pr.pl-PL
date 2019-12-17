---
title: Problemy z wydajnością-SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068422"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="5710e-102">SharePoint lub OneDrive powolne, niedostępne lub niedostępne dla wielu użytkowników</span><span class="sxs-lookup"><span data-stu-id="5710e-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="5710e-103">SharePoint lub OneDrive może być powolne, niedostępne lub niedostępne lub mogą być wyświetlane usługi niedostępne lub 503 błędy, z kilku powodów:</span><span class="sxs-lookup"><span data-stu-id="5710e-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="5710e-104">Jeśli witryny programu SharePoint lub OneDrive jest powolne lub opóźnione dla wielu użytkowników, może być problem tymczasowy usługi, gdzie użytkownicy wystąpić sporadyczne opóźnienia lub błędy nawigacji podczas uzyskiwania dostępu do witryn programu SharePoint lub zawartości OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5710e-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="5710e-105">Sprawdź [pulpit nawigacyjny kondycji usługi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , aby zobaczyć, jeśli Twoja organizacja ma wpływ.</span><span class="sxs-lookup"><span data-stu-id="5710e-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="5710e-106">Użytkownicy mogą otrzymać *503 serwer jest zajęty* błąd podczas próby przejdź do witryny programu SharePoint lub OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5710e-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="5710e-107">Ten błąd może być spowodowany przez ograniczanie przepustowości w ramach usługi programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5710e-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="5710e-108">Usługa SharePoint Online używa ograniczania przepustowości, aby zachować optymalną wydajność i niezawodność usługi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="5710e-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5710e-109">Ograniczanie ogranicza liczbę akcji użytkownika lub równoczesnych wywołań (przez skrypt lub kod), aby zapobiec nadmiernym użyciu zasobów.</span><span class="sxs-lookup"><span data-stu-id="5710e-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="5710e-110">Aby uzyskać więcej informacji na temat ograniczania przepustowości Zobacz, [Unikaj uzyskiwania ograniczane lub zablokowane w programie SharePoint w trybie online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="5710e-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="5710e-111">Jeśli wydajność pracy jest niska w **klasycznej** lub **nowoczesnej** witrynie lub na stronie programu SharePoint, użyj [narzędzia diagnostycznego strony](https://aka.ms/perftool) do analizowania stron.</span><span class="sxs-lookup"><span data-stu-id="5710e-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="5710e-112">Jeśli nadal występują ogólne niska wydajność, zapoznaj się z zasobami na dole tego artykułu: [wprowadzenie do dostrajania wydajności programu SharePoint w trybie online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="5710e-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  
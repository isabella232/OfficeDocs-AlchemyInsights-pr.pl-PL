---
title: Problemy z wydajnością — program SharePoint lub usługa OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771911"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="724db-102">Program SharePoint lub usługa OneDrive jest wolny, niedostępny lub niedostępny dla wielu użytkowników</span><span class="sxs-lookup"><span data-stu-id="724db-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="724db-103">Program SharePoint lub usługa OneDrive może być wolny, niedostępny lub niedostępny albo może wyświetlać niedostępną usługę lub 503 błędy z kilku powodów:</span><span class="sxs-lookup"><span data-stu-id="724db-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="724db-104">Jeśli witryna programu SharePoint lub usługi OneDrive jest powolna lub opóźniona dla wielu użytkowników, może to oznaczać, że wystąpił tymczasowy problem z usługą, w którym użytkownicy mogą napotkać sporadyczne opóźnienia lub błędy nawigacji podczas uzyskiwania dostępu do witryn programu SharePoint lub zawartości OneDrive.</span><span class="sxs-lookup"><span data-stu-id="724db-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="724db-105">Sprawdź [pulpit nawigacyjny kondycji usługi](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , aby sprawdzić, czy Twoja organizacja ma wpływ na.</span><span class="sxs-lookup"><span data-stu-id="724db-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="724db-106">Po próbie przejścia do witryny programu SharePoint lub usługi OneDrive użytkownicy mogą otrzymać komunikat o błędzie *serwera 503 jest zajęty* .</span><span class="sxs-lookup"><span data-stu-id="724db-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="724db-107">Przyczyną tego błędu może być ograniczenie w ramach usługi programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="724db-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="724db-108">Usługa SharePoint Online używa ograniczania, aby zapewnić optymalną wydajność i niezawodność usługi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="724db-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="724db-109">Ograniczanie ogranicza liczbę akcji użytkownika lub współbieżnych połączeń (za pomocą skryptu lub kodu), aby zapobiec nadmiernemu zużyciu zasobów.</span><span class="sxs-lookup"><span data-stu-id="724db-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="724db-110">Aby uzyskać więcej informacji na temat ograniczania przepustowości, zobacz [unikanie ograniczania lub blokowania w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="724db-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="724db-111">Jeśli masz niską wydajność w **klasycznej** lub **nowoczesnej** witrynie lub stronie programu SharePoint, użyj [narzędzia Diagnostyka strony](https://aka.ms/perftool) do analizowania stron.</span><span class="sxs-lookup"><span data-stu-id="724db-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="724db-112">Jeśli nadal masz ogólne wolne wyniki, zobacz zasoby na dole tego artykułu: [wprowadzenie do dostrajania wydajności usługi SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="724db-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  
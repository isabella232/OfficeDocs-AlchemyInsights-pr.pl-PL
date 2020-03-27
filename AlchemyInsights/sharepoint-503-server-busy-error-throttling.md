---
title: Ograniczanie przepustowości usługi SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958745"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="65f3b-102">Ograniczanie przepustowości usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="65f3b-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="65f3b-103">**Ważne:** W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostaną wysoce dostępne — odwiedź [witrynę SharePoint Online, aby](https://aka.ms/ODSPAdjustments) uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="65f3b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="65f3b-104">**Serwer 503 jest zajęty błąd**</span><span class="sxs-lookup"><span data-stu-id="65f3b-104">**503 server is busy error**</span></span>

<span data-ttu-id="65f3b-105">Użytkownicy mogą otrzymać błąd 503 serwer jest zajęty podczas próby przejścia do witryn programu SharePoint lub OneDrive.</span><span class="sxs-lookup"><span data-stu-id="65f3b-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="65f3b-106">Ten błąd może być spowodowany przez ograniczanie przepustowości w usłudze sharepoint.</span><span class="sxs-lookup"><span data-stu-id="65f3b-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="65f3b-107">Usługa SharePoint Online używa ograniczania przepustowości w celu zachowania optymalnej wydajności i niezawodności usługi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="65f3b-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="65f3b-108">Ograniczanie ogranicza liczbę akcji użytkownika lub równoczesnych wywołań (według skryptu lub kodu), aby zapobiec nadużywaniu zasobów.</span><span class="sxs-lookup"><span data-stu-id="65f3b-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="65f3b-109">Aby uzyskać więcej informacji na temat ograniczania przepustowości, [zobacz: Unikanie ograniczania lub blokowania w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="65f3b-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="65f3b-110">Jeśli uważasz, że ten błąd nie jest związany z ograniczaniem przepustowości, możesz sprawdzić, czy w dzierżawie występuje aktywna konserwacja, przechodząc do [Centrum wiadomości.](https://portal.office.com/adminportal/home#/MessageCenter)</span><span class="sxs-lookup"><span data-stu-id="65f3b-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="65f3b-111">Na koniec upewnij się, że odwiedź [service health](https://portal.office.com/adminportal/home#/servicehealth) strony, aby sprawdzić, czy wszelkie porady /incydenty, które mogą wystąpić.</span><span class="sxs-lookup"><span data-stu-id="65f3b-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>


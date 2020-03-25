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
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931236"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="2523c-102">Ograniczanie przepustowości usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2523c-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="2523c-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="2523c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2523c-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="2523c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2523c-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="2523c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2523c-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="2523c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2523c-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="2523c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2523c-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="2523c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2523c-109">**Serwer 503 jest zajęty błąd**</span><span class="sxs-lookup"><span data-stu-id="2523c-109">**503 server is busy error**</span></span>

<span data-ttu-id="2523c-110">Użytkownicy mogą otrzymać błąd 503 serwer jest zajęty podczas próby przejścia do witryn programu SharePoint lub OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2523c-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="2523c-111">Ten błąd może być spowodowany przez ograniczanie przepustowości w usłudze sharepoint.</span><span class="sxs-lookup"><span data-stu-id="2523c-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="2523c-112">Usługa SharePoint Online używa ograniczania przepustowości w celu zachowania optymalnej wydajności i niezawodności usługi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="2523c-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="2523c-113">Ograniczanie ogranicza liczbę akcji użytkownika lub równoczesnych wywołań (według skryptu lub kodu), aby zapobiec nadużywaniu zasobów.</span><span class="sxs-lookup"><span data-stu-id="2523c-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="2523c-114">Aby uzyskać więcej informacji na temat ograniczania przepustowości, [zobacz: Unikanie ograniczania lub blokowania w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="2523c-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="2523c-115">Jeśli uważasz, że ten błąd nie jest związany z ograniczaniem przepustowości, możesz sprawdzić, czy w dzierżawie występuje aktywna konserwacja, przechodząc do [Centrum wiadomości.](https://portal.office.com/adminportal/home#/MessageCenter)</span><span class="sxs-lookup"><span data-stu-id="2523c-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="2523c-116">Na koniec upewnij się, że odwiedź [service health](https://portal.office.com/adminportal/home#/servicehealth) strony, aby sprawdzić, czy wszelkie porady /incydenty, które mogą wystąpić.</span><span class="sxs-lookup"><span data-stu-id="2523c-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>


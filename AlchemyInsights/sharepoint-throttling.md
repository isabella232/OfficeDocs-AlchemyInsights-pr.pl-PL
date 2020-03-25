---
title: Ograniczanie przepustowości usługi SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931452"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="35620-102">Ograniczanie przepustowości usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="35620-102">SharePoint Online throttling</span></span>

<span data-ttu-id="35620-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="35620-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="35620-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="35620-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="35620-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="35620-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="35620-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="35620-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="35620-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="35620-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="35620-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="35620-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="35620-109">**Ograniczanie przepustowości usługi SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="35620-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="35620-110">Usługa SharePoint Online używa ograniczania przepustowości w celu zachowania optymalnej wydajności i niezawodności usługi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="35620-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="35620-111">Ograniczanie ogranicza liczbę akcji użytkownika lub równoczesnych wywołań (według skryptu lub kodu), aby zapobiec nadużywaniu zasobów.</span><span class="sxs-lookup"><span data-stu-id="35620-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="35620-112">Aby uzyskać więcej informacji, odwiedź poniższe linki.</span><span class="sxs-lookup"><span data-stu-id="35620-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="35620-113">Unikanie ograniczania lub blokowania w usłudze SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="35620-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="35620-114">Migracja danych i ograniczanie spo</span><span class="sxs-lookup"><span data-stu-id="35620-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="35620-115">Szybkość migracji w usłudze SharePoint Online i usłudze OneDrive</span><span class="sxs-lookup"><span data-stu-id="35620-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="35620-116">Obsługa ograniczania przepustowości usługi SharePoint Online przy użyciu wykładniczego wycofywania</span><span class="sxs-lookup"><span data-stu-id="35620-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="35620-117">Planowanie pojemności i testowanie obciążenia usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="35620-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)


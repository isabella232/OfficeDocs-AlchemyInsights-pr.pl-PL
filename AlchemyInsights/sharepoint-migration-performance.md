---
title: Wydajność migracji w programie SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932244"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="7a9b0-102">Wydajność migracji w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="7a9b0-102">SharePoint migration performance</span></span>

<span data-ttu-id="7a9b0-103">**Ważne**: wielu klientów usług SharePoint Online i OneDrive używa aplikacji o krytycznym znaczeniu, na które wpływają usługi wykonywane w tle.</span><span class="sxs-lookup"><span data-stu-id="7a9b0-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7a9b0-104">Obejmuje to rozwiązania do migracji treści, ochrony przed utratą danych (DLP) czy do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="7a9b0-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7a9b0-105">W tych bezprecedensowych czasach podejmujemy kroki mające na celu zapewnienie, że usługi SharePoint Online oraz OneDrive pozostają dostępne i działają niezawodnie dla użytkowników, którzy bardziej niż kiedykolwiek polegają na nich przy pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="7a9b0-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7a9b0-106">Aby móc realizować ten cel, wprowadziliśmy ściślejsze limity ograniczania dla aplikacji działających w tle (migracji, funkcji DLP i rozwiązań do tworzenia kopii zapasowych) w godzinach pracy w dni robocze.</span><span class="sxs-lookup"><span data-stu-id="7a9b0-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7a9b0-107">W tym czasie należy spodziewać się, że w tych godzinach aplikacje te uzyskają bardzo ograniczoną przepływność.</span><span class="sxs-lookup"><span data-stu-id="7a9b0-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7a9b0-108">Natomiast w godzinach wieczornych oraz w weekendy w danym regionie usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="7a9b0-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7a9b0-109">**Wydajność migracji**</span><span class="sxs-lookup"><span data-stu-id="7a9b0-109">**Migration performance**</span></span>

<span data-ttu-id="7a9b0-110">Na wydajność migracji może mieć wpływ infrastruktura sieciowa, rozmiar pliku, godzina przeprowadzania migracji czy ograniczanie.</span><span class="sxs-lookup"><span data-stu-id="7a9b0-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="7a9b0-111">Ich znajomość ułatwi Ci zaplanowanie migracji i zmaksymalizowanie jej wydajności.</span><span class="sxs-lookup"><span data-stu-id="7a9b0-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="7a9b0-112">Aby uzyskać więcej informacji, skorzystaj z poniższych linków.</span><span class="sxs-lookup"><span data-stu-id="7a9b0-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="7a9b0-113">Szybkość migracji usług SharePoint Online i OneDrive dla Firm</span><span class="sxs-lookup"><span data-stu-id="7a9b0-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="7a9b0-114">Unikanie ograniczania lub blokowania w usłudze SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7a9b0-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="7a9b0-115">Pobieranie i instalowanie narzędzia do migracji programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="7a9b0-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

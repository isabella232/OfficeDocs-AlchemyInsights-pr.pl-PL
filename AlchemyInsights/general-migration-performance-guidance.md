---
title: Ogólne wskazówki dotyczące wydajności migracji
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
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932488"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="966d6-102">Ogólne wskazówki dotyczące wydajności migracji</span><span class="sxs-lookup"><span data-stu-id="966d6-102">General migration performance guidance</span></span>

<span data-ttu-id="966d6-103">**Ważne**: wielu klientów usług SharePoint Online i OneDrive używa aplikacji o krytycznym znaczeniu, na które wpływają usługi wykonywane w tle.</span><span class="sxs-lookup"><span data-stu-id="966d6-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="966d6-104">Obejmuje to rozwiązania do migracji treści, ochrony przed utratą danych (DLP) czy do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="966d6-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="966d6-105">W tych bezprecedensowych czasach podejmujemy kroki mające na celu zapewnienie, że usługi SharePoint Online oraz OneDrive pozostają dostępne i działają niezawodnie dla użytkowników, którzy bardziej niż kiedykolwiek polegają na nich przy pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="966d6-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="966d6-106">Aby móc realizować ten cel, wprowadziliśmy ściślejsze limity ograniczania dla aplikacji działających w tle (migracji, funkcji DLP i rozwiązań do tworzenia kopii zapasowych) w godzinach pracy w dni robocze.</span><span class="sxs-lookup"><span data-stu-id="966d6-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="966d6-107">W tym czasie należy spodziewać się, że w tych godzinach aplikacje te uzyskają bardzo ograniczoną przepływność.</span><span class="sxs-lookup"><span data-stu-id="966d6-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="966d6-108">Natomiast w godzinach wieczornych oraz w weekendy w danym regionie usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="966d6-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="966d6-109">**Wskazówki dotyczące wydajności migracji**</span><span class="sxs-lookup"><span data-stu-id="966d6-109">**Migration performance guidance**</span></span>

<span data-ttu-id="966d6-110">Na wydajność migracji może mieć wpływ infrastruktura sieciowa, rozmiar pliku, godzina przeprowadzania migracji czy ograniczanie.</span><span class="sxs-lookup"><span data-stu-id="966d6-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="966d6-111">Zrozumienie tego ułatwi Ci zaplanowanie migracji i zapewnienie jej maksymalnej wydajności.</span><span class="sxs-lookup"><span data-stu-id="966d6-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="966d6-112">Ogólne wskazówki dotyczące wydajności migracji</span><span class="sxs-lookup"><span data-stu-id="966d6-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

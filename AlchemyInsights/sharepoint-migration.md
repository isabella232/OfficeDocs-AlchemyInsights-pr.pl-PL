---
title: Opcje migracji do usługi SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932740"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="0cd5f-102">Opcje migracji do usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="0cd5f-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="0cd5f-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="0cd5f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0cd5f-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="0cd5f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0cd5f-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="0cd5f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0cd5f-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="0cd5f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0cd5f-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="0cd5f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0cd5f-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="0cd5f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0cd5f-109">**Opcje migracji**</span><span class="sxs-lookup"><span data-stu-id="0cd5f-109">**Migration options**</span></span>

<span data-ttu-id="0cd5f-110">Istnieją różne opcje migracji zawartości do usługi SharePoint Online, w zależności od rozmiaru i ilości plików, które należy przenieść, zobacz listę opcji [znajdujących się tutaj](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="0cd5f-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="0cd5f-111">Aby uzyskać więcej informacji na temat migracji treści, odwiedź poniższe linki.</span><span class="sxs-lookup"><span data-stu-id="0cd5f-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="0cd5f-112">Narzędzie migracji programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="0cd5f-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="0cd5f-113">Wprowadzenie do Menedżera migracji</span><span class="sxs-lookup"><span data-stu-id="0cd5f-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="0cd5f-114">Szybkość migracji w usłudze Sharepoint Online i ODB</span><span class="sxs-lookup"><span data-stu-id="0cd5f-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="0cd5f-115">Unikanie ograniczania lub blokowania w usłudze SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="0cd5f-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="0cd5f-116">Narzędzie oceny migracji programu SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="0cd5f-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="0cd5f-117">**Uwaga:** Obecnie narzędzie Migracji programu SharePoint obsługuje tylko migracje z programu SharePoint 2010 i 2013.</span><span class="sxs-lookup"><span data-stu-id="0cd5f-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="0cd5f-118">Wersja 2016 lub 2019 nie są obecnie obsługiwane.</span><span class="sxs-lookup"><span data-stu-id="0cd5f-118">Version 2016 or 2019 are not supported at this time.</span></span>

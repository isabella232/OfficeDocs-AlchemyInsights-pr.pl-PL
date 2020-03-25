---
title: Problemy podczas migracji danych do usługi SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931704"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="136c9-102">Problemy podczas migracji danych do usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="136c9-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="136c9-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="136c9-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="136c9-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="136c9-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="136c9-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="136c9-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="136c9-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="136c9-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="136c9-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="136c9-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="136c9-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="136c9-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="136c9-109">**Migrowanie ponad 100 TB danych**</span><span class="sxs-lookup"><span data-stu-id="136c9-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="136c9-110">Wygląda na to, że migrujesz ponad 100 TB danych do usługi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="136c9-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="136c9-111">Postępuj zgodnie z poniższymi krokami, abyśmy mogli pomóc Ci tak szybko, jak to możliwe.</span><span class="sxs-lookup"><span data-stu-id="136c9-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="136c9-112">Wybierz **pozycję Nowe żądanie usługi**, a następnie pozycję Nowe żądanie **usługi**.</span><span class="sxs-lookup"><span data-stu-id="136c9-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="136c9-113">Pozostaw tytuł i opis jako **migracja programu SharePoint o masie ponad 100 TB.**</span><span class="sxs-lookup"><span data-stu-id="136c9-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="136c9-114">Po przesłaniu biletu należy go zaktualizować o następujące informacje:</span><span class="sxs-lookup"><span data-stu-id="136c9-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="136c9-115">Szacowany rozmiar migracji.</span><span class="sxs-lookup"><span data-stu-id="136c9-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="136c9-116">Oszacowanie, kiedy chcesz rozpocząć i zakończyć migrację.</span><span class="sxs-lookup"><span data-stu-id="136c9-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="136c9-117">Opisz miejsce migracji zawartości, takiej jak SharePoint Server, Box, GDrive, Udziały plików itp.</span><span class="sxs-lookup"><span data-stu-id="136c9-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  


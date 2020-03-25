---
title: Ograniczanie migracji programu SharePoint z 503 błędami
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931668"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="99032-102">Ograniczanie migracji programu SharePoint z 503 błędami</span><span class="sxs-lookup"><span data-stu-id="99032-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="99032-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="99032-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="99032-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="99032-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="99032-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="99032-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="99032-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="99032-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="99032-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="99032-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="99032-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="99032-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="99032-109">**503 błędy podczas migracji do usługi SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="99032-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="99032-110">Wygląda na to, że przeprowadzasz migrację do usługi SharePoint Online i otrzymujesz 503 błędy.</span><span class="sxs-lookup"><span data-stu-id="99032-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="99032-111">Postępuj zgodnie z poniższymi krokami, abyśmy mogli pomóc Ci tak szybko, jak to możliwe.</span><span class="sxs-lookup"><span data-stu-id="99032-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="99032-112">Kliknij **pozycję Skontaktuj się z pomocą techniczną**, a następnie pozycję Nowe żądanie **usługi**.</span><span class="sxs-lookup"><span data-stu-id="99032-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="99032-113">Aby uzyskać tytuł i opis, wpisz **dławienie migracji programu SharePoint z 503**.</span><span class="sxs-lookup"><span data-stu-id="99032-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="99032-114">Po przesłaniu biletu należy go zaktualizować o następujące informacje:</span><span class="sxs-lookup"><span data-stu-id="99032-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="99032-115">Ile pozostało z migracji (na przykład, ile TBs?).</span><span class="sxs-lookup"><span data-stu-id="99032-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="99032-116">Data rozpoczęcia i zakończenia migracji.</span><span class="sxs-lookup"><span data-stu-id="99032-116">Migration start and end date.</span></span>
    - <span data-ttu-id="99032-117">Opisz miejsce migracji zawartości, takiej jak SharePoint Server, Box, GDrive, Udziały plików itp.</span><span class="sxs-lookup"><span data-stu-id="99032-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="99032-118">Oszacuj liczbę błędów ograniczania przepustowości (na przykład x przepustnicy na godzinę?) i kiedy wystąpiło ograniczanie przepustowości.</span><span class="sxs-lookup"><span data-stu-id="99032-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="99032-119">Używane narzędzie do migracji (na przykład SPMT lub ShareGate).</span><span class="sxs-lookup"><span data-stu-id="99032-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>



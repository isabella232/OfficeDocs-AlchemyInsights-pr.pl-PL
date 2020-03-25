---
title: Rozwiązywanie problemów z narzędziem migracji programu SharePoint i błędów
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931128"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="e3e2e-102">Rozwiązywanie problemów z narzędziem migracji programu SharePoint i błędów</span><span class="sxs-lookup"><span data-stu-id="e3e2e-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="e3e2e-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="e3e2e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e3e2e-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="e3e2e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e3e2e-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="e3e2e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e3e2e-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="e3e2e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e3e2e-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="e3e2e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e3e2e-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="e3e2e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e3e2e-109">**Typowe problemy i błędy**</span><span class="sxs-lookup"><span data-stu-id="e3e2e-109">**Common issues and errors**</span></span>

<span data-ttu-id="e3e2e-110">Podczas korzystania z narzędzia sharepoint migration tool (SPMT) mogą wystąpić typowe problemy i błędy.</span><span class="sxs-lookup"><span data-stu-id="e3e2e-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="e3e2e-111">Aby uzyskać więcej informacji, zapoznaj się z poniższymi linkami.</span><span class="sxs-lookup"><span data-stu-id="e3e2e-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="e3e2e-112">Rozwiązywanie typowych problemów i błędów SPMT</span><span class="sxs-lookup"><span data-stu-id="e3e2e-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="e3e2e-113">Rozwiązywanie problemów z instalacją narzędzia SPMT</span><span class="sxs-lookup"><span data-stu-id="e3e2e-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)
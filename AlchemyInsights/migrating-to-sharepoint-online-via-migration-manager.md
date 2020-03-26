---
title: Migrowanie od usługi SharePoint za pośrednictwem Menedżera migracji
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932188"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="d7ed3-102">Migrowanie od usługi SharePoint za pośrednictwem Menedżera migracji</span><span class="sxs-lookup"><span data-stu-id="d7ed3-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="d7ed3-103">**Ważne**: wielu klientów usług SharePoint Online i OneDrive używa aplikacji o krytycznym znaczeniu, na które wpływają usługi wykonywane w tle.</span><span class="sxs-lookup"><span data-stu-id="d7ed3-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d7ed3-104">Obejmuje to rozwiązania do migracji treści, ochrony przed utratą danych (DLP) czy do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="d7ed3-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d7ed3-105">W tych bezprecedensowych czasach podejmujemy kroki mające na celu zapewnienie, że usługi SharePoint Online oraz OneDrive pozostają dostępne i działają niezawodnie dla użytkowników, którzy bardziej niż kiedykolwiek polegają na nich przy pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="d7ed3-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d7ed3-106">Aby móc realizować ten cel, wprowadziliśmy ściślejsze limity ograniczania dla aplikacji działających w tle (migracji, funkcji DLP i rozwiązań do tworzenia kopii zapasowych) w godzinach pracy w dni robocze.</span><span class="sxs-lookup"><span data-stu-id="d7ed3-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d7ed3-107">W tym czasie należy spodziewać się, że w tych godzinach aplikacje te uzyskają bardzo ograniczoną przepływność.</span><span class="sxs-lookup"><span data-stu-id="d7ed3-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d7ed3-108">Natomiast w godzinach wieczornych oraz w weekendy w danym regionie usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="d7ed3-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d7ed3-109">**Menedżer migracji**</span><span class="sxs-lookup"><span data-stu-id="d7ed3-109">**Migration Manager**</span></span>

<span data-ttu-id="d7ed3-110">Menedżer migracji dostępny w nowoczesnym centrum administracyjnym programu SharePoint przeprowadzi Cię przez proces konfigurowania klientów i tworzenia zadań.</span><span class="sxs-lookup"><span data-stu-id="d7ed3-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="d7ed3-111">Za jego pomocą możesz skonfigurować ustawienia globalne i dotyczące poszczególnych zadań, wyświetlić postępy w realizacji wszystkich zadań i pobrać zagregowane podsumowanie i raporty dotyczące zadań.</span><span class="sxs-lookup"><span data-stu-id="d7ed3-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="d7ed3-112">Wprowadzenie do Menadżera migracji</span><span class="sxs-lookup"><span data-stu-id="d7ed3-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="d7ed3-113">Konfiguracja klientów Menadżera migracji</span><span class="sxs-lookup"><span data-stu-id="d7ed3-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- <span data-ttu-id="d7ed3-114">[Ustawienia Menadżera migracji</span><span class="sxs-lookup"><span data-stu-id="d7ed3-114">[Migration Manager Settings](https://docs.microsoft.com/sharepointmigration/mm-settings)</span></span>

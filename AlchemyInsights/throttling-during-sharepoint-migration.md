---
title: Ograniczanie podczas migracji w programie SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958908"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="ae88c-102">Ograniczanie w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="ae88c-102">SharePoint throttling</span></span>

<span data-ttu-id="ae88c-103">**Ważne**: W tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="ae88c-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ae88c-104">**Ograniczanie w usłudze SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="ae88c-104">**SharePoint Online throttling**</span></span>

<span data-ttu-id="ae88c-105">Usługa SharePoint Online używa ograniczania, aby zapewnić optymalną wydajność i niezawodność usługi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ae88c-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="ae88c-106">Ograniczanie ogranicza liczbę akcji użytkownika lub współbieżnych połączeń (za pomocą skryptu lub kodu), aby zapobiec nadmiernemu zużyciu zasobów.</span><span class="sxs-lookup"><span data-stu-id="ae88c-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="ae88c-107">Aby uzyskać więcej informacji, skorzystaj z poniższych linków:</span><span class="sxs-lookup"><span data-stu-id="ae88c-107">For more information please visit the links below:</span></span>

- [<span data-ttu-id="ae88c-108">Unikanie ograniczania lub blokowania w usłudze SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ae88c-108">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [<span data-ttu-id="ae88c-109">Migracja danych i ograniczanie SPO</span><span class="sxs-lookup"><span data-stu-id="ae88c-109">Data Migration and SPO Throttling</span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [<span data-ttu-id="ae88c-110">Szybkość migracji usług SharePoint Online i OneDrive</span><span class="sxs-lookup"><span data-stu-id="ae88c-110">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- [<span data-ttu-id="ae88c-111">Obsługa ograniczania usługi SharePoint Online przy użyciu wykładniczej funkcji wycofywania</span><span class="sxs-lookup"><span data-stu-id="ae88c-111">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [<span data-ttu-id="ae88c-112">Planowanie wydajności i testowanie obciążenia usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ae88c-112">Capacity planning and load testing SharePoint Online</span></span>](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)
- [<span data-ttu-id="ae88c-113">Podczas migracji występuje niska wydajność lub ograniczanie</span><span class="sxs-lookup"><span data-stu-id="ae88c-113">I am experiencing poor performance or throttling during migration</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)
---
title: Brakuje spisu oprogramowania lub niedokładne informacje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676510"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="d582b-102">Brakuje spisu oprogramowania lub niedokładne informacje</span><span class="sxs-lookup"><span data-stu-id="d582b-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="d582b-103">Spis oprogramowania w aplikacji Zarządzanie zagrożeniami i lukami to lista znanego oprogramowania w organizacji z oficjalnymi wyliczeniami wspólnej platformy (CPE, Common Platform Enumerations).</span><span class="sxs-lookup"><span data-stu-id="d582b-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="d582b-104">Produkty oprogramowania bez oficjalnego cpe nie mają opublikowanych luk w zabezpieczeniach.</span><span class="sxs-lookup"><span data-stu-id="d582b-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="d582b-105">W spisie znajdują się również szczegółowe informacje, takie jak imię i nazwisko dostawcy, liczba braków, zagrożenia i liczba dostępnych urządzeń.</span><span class="sxs-lookup"><span data-stu-id="d582b-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="d582b-106">Zmiany oprogramowania na urządzeniach są zazwyczaj odzwierciedlane w portalach zabezpieczeń w ciągu dwóch godzin.</span><span class="sxs-lookup"><span data-stu-id="d582b-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="d582b-107">Jednak czasami może to trwać dłużej.</span><span class="sxs-lookup"><span data-stu-id="d582b-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="d582b-108">Obecnie nie można wymusić synchronizacji. jest to ciągła ocena.</span><span class="sxs-lookup"><span data-stu-id="d582b-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="d582b-109">Jeśli po 5 godzinach zmiany oprogramowania w programie tvm nie są dokładnie odzwierciedlane, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="d582b-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="d582b-110">Zapoznaj się z sekcją dowodów na temat oprogramowania, aby dowiedzieć się, jak wykryto oprogramowanie.</span><span class="sxs-lookup"><span data-stu-id="d582b-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="d582b-111">Upewnij się, że oprogramowanie jest obsługiwane.</span><span class="sxs-lookup"><span data-stu-id="d582b-111">Make sure that the software is supported.</span></span> <span data-ttu-id="d582b-112">Oprogramowanie może być widoczne tylko na poziomie urządzenia, nawet jeśli nie jest obecnie obsługiwane przez Zarządzanie zagrożeniami i lukami.</span><span class="sxs-lookup"><span data-stu-id="d582b-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="d582b-113">Dostępne są jednak tylko ograniczone dane.</span><span class="sxs-lookup"><span data-stu-id="d582b-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="d582b-114">Aby uzyskać instrukcje dotyczące zgłaszania nieścisłości z portalu, zobacz Zgłaszanie [nieścisłości.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="d582b-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="d582b-115">**Uwaga:** Zgłaszanie nieścisłości z portalu MDE to jednokierunkowy kanał dla inżynierów.</span><span class="sxs-lookup"><span data-stu-id="d582b-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="d582b-116">Jeśli ten problem jest pilny, otwórz bilet pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="d582b-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="d582b-117">Aby uzyskać więcej informacji, zobacz [Spis Zarządzanie zagrożeniami i lukami.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)</span><span class="sxs-lookup"><span data-stu-id="d582b-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>
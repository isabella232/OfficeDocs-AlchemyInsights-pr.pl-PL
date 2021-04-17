---
title: Brak wyników wyszukiwania zawartości
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816858"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="56c3c-102">Brak wyników wyszukiwania/eksportu zawartości</span><span class="sxs-lookup"><span data-stu-id="56c3c-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="56c3c-103">Problemy z wyszukiwaniem/eksportem zawartości, które nie zwracają żadnych danych, mogą być spowodowane pewnym filtrem zabezpieczeń zgodności, który został określony przez określonego administratora i nie jest przekazywania go wszystkim administratorom.</span><span class="sxs-lookup"><span data-stu-id="56c3c-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="56c3c-104">Aby rozwiązać ten problem, sprawdź, czy istnieją filtry zabezpieczeń zgodności, które mogą być przyczyną tego problemu:</span><span class="sxs-lookup"><span data-stu-id="56c3c-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="56c3c-105">Nawiązywanie połączenia z Centrum zabezpieczeń i zgodności w programie PowerShell</span><span class="sxs-lookup"><span data-stu-id="56c3c-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="56c3c-106">Uruchom następujące polecenia:</span><span class="sxs-lookup"><span data-stu-id="56c3c-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="56c3c-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="56c3c-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="56c3c-108">Get-ComplianceSecurityFilter — Organizacja $org</span><span class="sxs-lookup"><span data-stu-id="56c3c-108">Get-ComplianceSecurityFilter -Organization $org</span></span>
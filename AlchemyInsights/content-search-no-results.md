---
title: Nie wyników wyszukiwania zawartości
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516789"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="65363-102">Brak wyników z zawartości wyszukiwania/wywozu</span><span class="sxs-lookup"><span data-stu-id="65363-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="65363-103">Problemy z zawartości wyszukiwania/wywozu nie zwróciła żadnych danych może być spowodowane niektórych zgodności filtr zabezpieczeń, który został skonfigurowany przez administratora konkretnego i nie komunikuje się wszyscy administratorzy.</span><span class="sxs-lookup"><span data-stu-id="65363-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="65363-104">Aby rozwiązać ten problem, sprawdź, czy są wszystkie filtry zabezpieczeń zgodności, która może być przyczyną tego:</span><span class="sxs-lookup"><span data-stu-id="65363-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="65363-105">Podłącz do bezpieczeństwa i środowiska Powershell Centrum zgodności</span><span class="sxs-lookup"><span data-stu-id="65363-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="65363-106">Uruchom następujące aplety poleceń środowiska:</span><span class="sxs-lookup"><span data-stu-id="65363-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="65363-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="65363-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="65363-108">Get-ComplianceSecurityFilter-organizacja $org</span><span class="sxs-lookup"><span data-stu-id="65363-108">Get-ComplianceSecurityFilter -Organization $org</span></span>
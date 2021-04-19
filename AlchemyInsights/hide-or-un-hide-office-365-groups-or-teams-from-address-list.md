---
title: Ukrywanie lub ukrywanie grup lub zespołów usługi Office 365 na liście adresów
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811466"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="5a37e-102">Ukrywanie lub ukrywanie grup lub zespołów usługi Office 365 na liście adresów</span><span class="sxs-lookup"><span data-stu-id="5a37e-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="5a37e-103">Za pomocą następującego polecenia programu PowerShell programu EXO ukryj lub ukryj grupy/zespoły usługi Office 365 na listach adresowych (GAL) klientów programu Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="5a37e-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="5a37e-104">Aby ukryć lub ukryć grupy/zespoły usługi Office365 w klientach programu Exchange (Outlook, OWA), użyj następującego polecenia programu POWERShell programu EXO:</span><span class="sxs-lookup"><span data-stu-id="5a37e-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="5a37e-105">Aby uzyskać szczegółowe instrukcje, [zobacz Ukrywanie grup usługi Office 365 przed galą galp](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)i klientami programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a37e-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>

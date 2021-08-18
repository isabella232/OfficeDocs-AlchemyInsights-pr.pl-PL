---
title: Ukrywanie lub ukrywanie Office 365 lub zespołów na liście adresów
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088406"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Ukrywanie lub ukrywanie Office 365 lub zespołów na liście adresów

Za pomocą następującego polecenia programu PowerShell programu EXO można ukrywać lub ukrywać Office 365/zespoły na listach adresowych (GAL) klientów programu Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Użyj następującego polecenia programu PowerShell programu EXO, aby ukryć lub ukryć grupę/zespoły usługi Office365 w klientach Exchange klientach (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Aby uzyskać szczegółowe instrukcje, zobacz [Ukrywanie Office 365 na galp i Exchange klientach.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)

---
title: Instrukcje ukrywania/odkrywania grupy z listy adresów
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908354"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ukrywanie grupy usługi Microsoft 365 z listy adresów (GAL)

Aby ukryć grupę usługi Microsoft 365 przed listami adresów (GAL) klientów programu Exchange (takich jak Outlook lub OWA), użyj następującego polecenia w powłoce EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Aby ukryć, że grupa usługi Microsoft 365 nie jest widoczna dla klientów programu Exchange, użyj następującego polecenia w powłoce EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


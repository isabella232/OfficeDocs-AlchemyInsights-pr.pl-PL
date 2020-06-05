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
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580019"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ukrywanie grupy usługi Microsoft 365 z listy adresów (GAL)

Aby ukryć grupę usługi Microsoft 365 przed listami adresów (GAL) klientów programu Exchange (takich jak Outlook lub OWA), użyj następującego polecenia w powłoce EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Aby ukryć, że grupa usługi Microsoft 365 nie jest widoczna dla klientów programu Exchange, użyj następującego polecenia w powłoce EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


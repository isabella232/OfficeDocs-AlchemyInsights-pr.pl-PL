---
title: Instrukcje ukrywania/odkrywania grup na liście adresów
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663019"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ukrywanie grupy programu Microsoft 365 z listy adresowej

Aby ukryć grupę Microsoft 365 z poziomu list adresowych (EXO) klientów programu Exchange (takich jak Outlook lub OWA), użyj następującego polecenia w powłoce:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Aby ukryć grupę Microsoft 365, która jest widoczna dla klientów programu Exchange, użyj następującego polecenia w powłoce EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


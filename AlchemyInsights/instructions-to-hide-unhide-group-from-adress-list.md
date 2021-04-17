---
title: Instrukcje ukrywania/odkrywania grupy na liście adresów
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
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831888"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ukrywanie grupy platformy Microsoft 365 na liście adresów (GAL)

Aby ukryć grupę platformy Microsoft 365 przed listami adresów (GAL) klientów programu Exchange (na przykład programu Outlook lub aplikacji OWA), użyj następującego polecenia w powłoki programu EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Aby ukryć grupę platformy Microsoft 365, aby nie była widoczna dla klientów programu Exchange, użyj następującego polecenia w powłoki EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


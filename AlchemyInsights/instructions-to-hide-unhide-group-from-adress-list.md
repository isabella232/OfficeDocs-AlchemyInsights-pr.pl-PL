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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926255"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ukrywanie Microsoft 365 na liście adresów (GAL)

Aby ukryć grupę Microsoft 365 na listach adresowych (GAL) klientów usługi Exchange (takich jak Outlook lub OWA), użyj następującego polecenia w powłoki exo:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Aby ukryć grupę Microsoft 365, aby była widoczna Exchange klientów, użyj następującego polecenia w powłoki EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


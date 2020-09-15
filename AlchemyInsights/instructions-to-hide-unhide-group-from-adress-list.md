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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="876a1-102">Ukrywanie grupy programu Microsoft 365 z listy adresowej</span><span class="sxs-lookup"><span data-stu-id="876a1-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="876a1-103">Aby ukryć grupę Microsoft 365 z poziomu list adresowych (EXO) klientów programu Exchange (takich jak Outlook lub OWA), użyj następującego polecenia w powłoce:</span><span class="sxs-lookup"><span data-stu-id="876a1-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="876a1-104">Aby ukryć grupę Microsoft 365, która jest widoczna dla klientów programu Exchange, użyj następującego polecenia w powłoce EXO:</span><span class="sxs-lookup"><span data-stu-id="876a1-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


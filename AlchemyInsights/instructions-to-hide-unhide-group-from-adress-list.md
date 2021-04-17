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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="86758-102">Ukrywanie grupy platformy Microsoft 365 na liście adresów (GAL)</span><span class="sxs-lookup"><span data-stu-id="86758-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="86758-103">Aby ukryć grupę platformy Microsoft 365 przed listami adresów (GAL) klientów programu Exchange (na przykład programu Outlook lub aplikacji OWA), użyj następującego polecenia w powłoki programu EXO:</span><span class="sxs-lookup"><span data-stu-id="86758-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="86758-104">Aby ukryć grupę platformy Microsoft 365, aby nie była widoczna dla klientów programu Exchange, użyj następującego polecenia w powłoki EXO:</span><span class="sxs-lookup"><span data-stu-id="86758-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


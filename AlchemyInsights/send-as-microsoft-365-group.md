---
title: Wyślij jako grupę Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872030"
---
# <a name="send-as-microsoft-365-group"></a>Wyślij jako grupę Microsoft 365

Możesz przypisać uprawnienia Wyślij jako, aby zezwolić określonym użytkownikom na wysyłanie wiadomości jako grupy programu Microsoft 365:  

1. Nawiązywanie połączenia z programem Exchange Online PowerShell.  

2. Uruchom następujące polecenie:  

    Add-RecipientPermission `<GroupName>` -powiernik `<MailboxName>` -AccessRights SendAs

Aby uzyskać więcej informacji, zobacz [Zezwalanie członkom na wysyłanie wiadomości jako lub wysyłanie w imieniu grupy](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).
---
title: Wiadomości wysyłane do grupy usługi Microsoft 365 nie są odbierane przez wszystkich członków
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480693"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Wiadomości wysyłane do grupy usługi Microsoft 365 nie są odbierane przez wszystkich członków

Upewnij się, że wszyscy członkowie grupy subskrybują wiadomości e-mail. Zobacz [Obserwowanie grupy w aplikacji Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Aby sprawdzić stan wiadomości członków, którzy zasubskrybowali grupowe wiadomości e-mail, uruchom następujące polecenie w [usłudze EXO programu PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Użyj następującego polecenia EXO programu PowerShell, aby skonfigurować odbieranie wiadomości e-mail wysyłanych do grupy usługi Microsoft 365 w skrzynkach odbiorczych wszystkich członków:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Przykład:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`
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
ms.openlocfilehash: 39a4f8115a4742947b3e6394396be5ce3b01e772
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430693"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="fc43f-102">Wiadomości wysyłane do grupy usługi Microsoft 365 nie są odbierane przez wszystkich członków</span><span class="sxs-lookup"><span data-stu-id="fc43f-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="fc43f-103">Upewnij się, że wszyscy członkowie grupy subskrybują wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="fc43f-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="fc43f-104">Zobacz [Obserwowanie grupy w aplikacji Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="fc43f-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="fc43f-105">Aby sprawdzić stan wiadomości członków, którzy zasubskrybowali grupowe wiadomości e-mail, uruchom następujące polecenie w [usłudze EXO programu PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="fc43f-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="fc43f-106">Użyj następującego polecenia EXO programu PowerShell, aby skonfigurować odbieranie wiadomości e-mail wysyłanych do grupy usługi Microsoft 365 w skrzynkach odbiorczych wszystkich członków:</span><span class="sxs-lookup"><span data-stu-id="fc43f-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`
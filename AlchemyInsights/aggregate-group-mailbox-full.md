---
title: AggregateGroupMailbox pełny raport NDR odebrany w przypadku wiadomości e-mail wysyłanych do grupy Microsoft 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722085"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a><span data-ttu-id="cdfd3-102">AggregateGroupMailbox pełny raport NDR odebrany w przypadku wiadomości e-mail wysyłanych do grupy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cdfd3-102">AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group</span></span>

<span data-ttu-id="cdfd3-103">Użyj następującego polecenia powłoki EXO, aby utworzyć regułę transportu programu Exchange w celu cichego porzucania wiadomości e-mail wysyłanych do grupowej skrzynki pocztowej grupy:</span><span class="sxs-lookup"><span data-stu-id="cdfd3-103">Use the following EXO Shell command to create an Exchange transport rule to silently drop emails sent to aggregate group mailbox:</span></span>

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> <span data-ttu-id="cdfd3-104">Zamień adres SMTP in **-SentTo** na adres SMTP zagregowanej skrzynki pocztowej grupy w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="cdfd3-104">Replace the SMTP address in **-SentTo** with SMTP address of aggregate group mailbox in your tenant.</span></span> <span data-ttu-id="cdfd3-105">Możesz uzyskać adres SMTP zagregowanej skrzynki pocztowej grupy z otrzymanego raportu o niedostarczeniu.</span><span class="sxs-lookup"><span data-stu-id="cdfd3-105">You can get the SMTP address of aggregate group mailbox from the NDR received.</span></span>




---
title: Błąd wysyłania wiadomości e-mail zablokowanych przez usługę SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813734"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="030f1-102">Błąd wysyłania wiadomości e-mail: Host klienta zablokowany przy użyciu usługi Spamhaus</span><span class="sxs-lookup"><span data-stu-id="030f1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="030f1-103">Adres IP, z który wysłano wiadomość, znajduje się na liście zablokowanych usługi [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="030f1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="030f1-104">Przykładowe powody zablokowania przez usługę Spamhaus to naruszone konta, naruszone komputery współużytkowanie publicznego adresu IP i zasady usługodawcy internetowego.</span><span class="sxs-lookup"><span data-stu-id="030f1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="030f1-105">Możliwe rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="030f1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="030f1-106">W przypadku zablokowanych wiadomości przychodzących, w których kontrolujesz źródłowy serwer poczty e-mail, musisz ustalić przyczynę i usunąć blokadę z witryny usługi Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="030f1-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="030f1-107">W przypadku zablokowanych wiadomości przychodzących, gdy źródłowy adres IP należy do innej osoby, właściciel adresu musi usunąć blokadę z witryny usługi Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="030f1-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="030f1-108">Jeśli adres IP znajduje się na liście blokad zasad (PBL, Policy Block List), właściciel może przypisać inny statyczny adres IP lub usunąć adres z listy blokad zasad.</span><span class="sxs-lookup"><span data-stu-id="030f1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="030f1-109">W przypadku zablokowanych wiadomości wychodzących z Twojej domeny połączonej z firmą Microsoft ten błąd może zostać wyświetlony, jeśli wiadomości są kierowane za pośrednictwem usługi innej firmy.</span><span class="sxs-lookup"><span data-stu-id="030f1-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="030f1-110">Aby znaleźć właściciela zablokowanego adresu IP, możesz użyć narzędzia wyszukiwania WHOIS.</span><span class="sxs-lookup"><span data-stu-id="030f1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>

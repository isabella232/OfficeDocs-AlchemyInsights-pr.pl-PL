---
title: Błąd podczas wysyłania wiadomości e-mail zablokowany przez SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714268"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="675e6-102">Błąd podczas wysyłania wiadomości e-mail: Host klienta zablokowany za pomocą spamhausu</span><span class="sxs-lookup"><span data-stu-id="675e6-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="675e6-103">Adres IP, który wysłał wiadomość, znajduje się na liście zablokowanych należącej do [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="675e6-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="675e6-104">Przyczyny zablokowania przez spamhaus obejmują przejęte konta, przejęte maszyny udostępniające publiczny adres IP oraz zasady dostawcy usług internetowych (ISP).</span><span class="sxs-lookup"><span data-stu-id="675e6-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="675e6-105">Możliwe poprawki to:</span><span class="sxs-lookup"><span data-stu-id="675e6-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="675e6-106">W przypadku zablokowanych wiadomości przychodzących, w których użytkownik kontroluje źródłowy serwer poczty e-mail, należy ustalić przyczynę i usunąć blok ze strony internetowej Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="675e6-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="675e6-107">W przypadku zablokowanych wiadomości przychodzących, w których źródłowy adres IP należy do innej osoby, właściciel adresu musi usunąć blok ze strony internetowej Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="675e6-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="675e6-108">Jeśli adres IP znajduje się na liście blokowania zasad (PBL), właściciel może przypisać inny statyczny adres IP lub usunąć adres z PBL.</span><span class="sxs-lookup"><span data-stu-id="675e6-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="675e6-109">W przypadku zablokowanych wiadomości wychodzących z domeny połączonej z firmą Microsoft ten błąd może być wyświetlony, jeśli wiadomości są kierowane za pośrednictwem usługi innej firmy.</span><span class="sxs-lookup"><span data-stu-id="675e6-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="675e6-110">Można użyć narzędzia wyszukiwania WHOIS, aby znaleźć zablokowanego właściciela adresu IP.</span><span class="sxs-lookup"><span data-stu-id="675e6-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>

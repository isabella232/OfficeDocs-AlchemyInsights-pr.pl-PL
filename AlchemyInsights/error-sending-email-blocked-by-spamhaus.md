---
title: Błąd podczas wysyłania wiadomości e-mail zablokowanej przez SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783813"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="7d7f6-102">Błąd podczas wysyłania wiadomości e-mail: Host klienta zablokowany przy użyciu Spamhaus</span><span class="sxs-lookup"><span data-stu-id="7d7f6-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="7d7f6-103">Adres IP, który wysłał wiadomość, znajduje się na liście zablokowanych należącej do [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="7d7f6-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="7d7f6-104">Powody do zablokowania przez Spamhaus obejmują złamane konta, a zagrożone komputery udostępniają publiczny adres IP oraz zasady usługodawcy internetowego (ISP).</span><span class="sxs-lookup"><span data-stu-id="7d7f6-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="7d7f6-105">Możliwe rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="7d7f6-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="7d7f6-106">W przypadku zablokowanych wiadomości przychodzących, w których kontroluje się źródłowy serwer poczty e-mail, należy określić przyczynę i usunąć blok z witryny internetowej spamhaus.</span><span class="sxs-lookup"><span data-stu-id="7d7f6-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="7d7f6-107">W przypadku zablokowanych wiadomości przychodzących, gdy źródłowy adres IP należy do innej osoby, właściciel adresu musi usunąć blok z witryny internetowej spamhaus.</span><span class="sxs-lookup"><span data-stu-id="7d7f6-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="7d7f6-108">Jeśli adres IP znajduje się na liście bloków zasad (PBL), właściciel może przypisać inny statyczny adres IP lub usunąć adres z PBL.</span><span class="sxs-lookup"><span data-stu-id="7d7f6-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="7d7f6-109">W przypadku zablokowanych wiadomości wychodzących z domeny połączonej z firmą Microsoft ten błąd może wystąpić, jeśli wiadomości są routowane za pośrednictwem usługi innej firmy.</span><span class="sxs-lookup"><span data-stu-id="7d7f6-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="7d7f6-110">Aby znaleźć zablokowanego właściciela adresu IP, możesz użyć narzędzia do wyszukiwania Whois Search Results.</span><span class="sxs-lookup"><span data-stu-id="7d7f6-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>

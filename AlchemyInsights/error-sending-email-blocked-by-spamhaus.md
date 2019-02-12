---
title: Wystąpił błąd podczas wysyłania wiadomości e-mail zablokowanych przez SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912358"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="4c52e-102">Wystąpił błąd podczas wysyłania poczty e-mail: klient host blokowane przy użyciu Spamhaus</span><span class="sxs-lookup"><span data-stu-id="4c52e-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="4c52e-p101">Adres IP, który wysłał wiadomość jest na liście zablokowanych posiadanych przez [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Powody blokowana przez Spamhaus obejmują dotyczących konta, zagrożone maszyn dzielenie publiczny adres IP, a zasady dostawcy usług internetowych (ISP). Ewentualnych poprawek są:</span><span class="sxs-lookup"><span data-stu-id="4c52e-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="4c52e-106">Zablokowane wiadomości przychodzących do której Kontrola źródłowego serwera e-mail usługi Office 365 należy ustalić przyczynę i Usuń blok z Spamhaus witryny sieci Web.</span><span class="sxs-lookup"><span data-stu-id="4c52e-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="4c52e-p102">Zablokowane wiadomości przychodzących do usługi Office 365, gdy źródłowy adres IP należy do kogoś innego właściciel adres musi blokada została usunięta z witryny Spamhaus. Jeśli adres IP jest na liście bloku zasad (PBL), właściciel można przypisać różne statyczny adres IP lub usunąć adres z PBL.</span><span class="sxs-lookup"><span data-stu-id="4c52e-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="4c52e-p103">Zablokowane wiadomości wychodzących z domeny usługi Office 365 można otrzymać ten błąd, jeśli wiadomości są routowane przez 3 usługa firmy. Można użyć narzędzia wyszukiwania WHOIS odnaleźć właściciela zablokowanych adresów IP.</span><span class="sxs-lookup"><span data-stu-id="4c52e-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    


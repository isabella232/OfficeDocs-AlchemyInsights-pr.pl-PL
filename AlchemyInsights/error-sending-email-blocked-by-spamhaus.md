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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Błąd wysyłania wiadomości e-mail: Host klienta zablokowany przy użyciu usługi Spamhaus

Adres IP, z który wysłano wiadomość, znajduje się na liście zablokowanych usługi [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) Przykładowe powody zablokowania przez usługę Spamhaus to naruszone konta, naruszone komputery współużytkowanie publicznego adresu IP i zasady usługodawcy internetowego. Możliwe rozwiązania:
  
- W przypadku zablokowanych wiadomości przychodzących, w których kontrolujesz źródłowy serwer poczty e-mail, musisz ustalić przyczynę i usunąć blokadę z witryny usługi Spamhaus.

- W przypadku zablokowanych wiadomości przychodzących, gdy źródłowy adres IP należy do innej osoby, właściciel adresu musi usunąć blokadę z witryny usługi Spamhaus. Jeśli adres IP znajduje się na liście blokad zasad (PBL, Policy Block List), właściciel może przypisać inny statyczny adres IP lub usunąć adres z listy blokad zasad.

- W przypadku zablokowanych wiadomości wychodzących z Twojej domeny połączonej z firmą Microsoft ten błąd może zostać wyświetlony, jeśli wiadomości są kierowane za pośrednictwem usługi innej firmy. Aby znaleźć właściciela zablokowanego adresu IP, możesz użyć narzędzia wyszukiwania WHOIS.

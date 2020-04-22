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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Błąd podczas wysyłania wiadomości e-mail: Host klienta zablokowany za pomocą spamhausu

Adres IP, który wysłał wiadomość, znajduje się na liście zablokowanych należącej do [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Przyczyny zablokowania przez spamhaus obejmują przejęte konta, przejęte maszyny udostępniające publiczny adres IP oraz zasady dostawcy usług internetowych (ISP). Możliwe poprawki to:
  
- W przypadku zablokowanych wiadomości przychodzących, w których użytkownik kontroluje źródłowy serwer poczty e-mail, należy ustalić przyczynę i usunąć blok ze strony internetowej Spamhaus.

- W przypadku zablokowanych wiadomości przychodzących, w których źródłowy adres IP należy do innej osoby, właściciel adresu musi usunąć blok ze strony internetowej Spamhaus. Jeśli adres IP znajduje się na liście blokowania zasad (PBL), właściciel może przypisać inny statyczny adres IP lub usunąć adres z PBL.

- W przypadku zablokowanych wiadomości wychodzących z domeny połączonej z firmą Microsoft ten błąd może być wyświetlony, jeśli wiadomości są kierowane za pośrednictwem usługi innej firmy. Można użyć narzędzia wyszukiwania WHOIS, aby znaleźć zablokowanego właściciela adresu IP.

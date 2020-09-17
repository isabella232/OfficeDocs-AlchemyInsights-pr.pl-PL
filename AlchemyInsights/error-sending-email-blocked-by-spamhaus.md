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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Błąd podczas wysyłania wiadomości e-mail: Host klienta zablokowany przy użyciu Spamhaus

Adres IP, który wysłał wiadomość, znajduje się na liście zablokowanych należącej do [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Powody do zablokowania przez Spamhaus obejmują złamane konta, a zagrożone komputery udostępniają publiczny adres IP oraz zasady usługodawcy internetowego (ISP). Możliwe rozwiązania:
  
- W przypadku zablokowanych wiadomości przychodzących, w których kontroluje się źródłowy serwer poczty e-mail, należy określić przyczynę i usunąć blok z witryny internetowej spamhaus.

- W przypadku zablokowanych wiadomości przychodzących, gdy źródłowy adres IP należy do innej osoby, właściciel adresu musi usunąć blok z witryny internetowej spamhaus. Jeśli adres IP znajduje się na liście bloków zasad (PBL), właściciel może przypisać inny statyczny adres IP lub usunąć adres z PBL.

- W przypadku zablokowanych wiadomości wychodzących z domeny połączonej z firmą Microsoft ten błąd może wystąpić, jeśli wiadomości są routowane za pośrednictwem usługi innej firmy. Aby znaleźć zablokowanego właściciela adresu IP, możesz użyć narzędzia do wyszukiwania Whois Search Results.

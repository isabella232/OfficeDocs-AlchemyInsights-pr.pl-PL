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
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402269"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Wystąpił błąd podczas wysyłania poczty e-mail: klient host blokowane przy użyciu Spamhaus

Adres IP, który wysłał wiadomość jest na liście zablokowanych posiadanych przez [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Powody blokowana przez Spamhaus obejmują dotyczących konta, zagrożone maszyn dzielenie publiczny adres IP, a zasady dostawcy usług internetowych (ISP). Ewentualnych poprawek są:
  
- Zablokowane wiadomości przychodzących do której Kontrola źródłowego serwera e-mail usługi Office 365 należy ustalić przyczynę i Usuń blok z Spamhaus witryny sieci Web.
    
- Zablokowane wiadomości przychodzących do usługi Office 365, gdy źródłowy adres IP należy do kogoś innego właściciel adres musi blokada została usunięta z witryny Spamhaus. Jeśli adres IP jest na liście bloku zasad (PBL), właściciel można przypisać różne statyczny adres IP lub usunąć adres z PBL.
    
- Zablokowane wiadomości wychodzących z domeny usługi Office 365 można otrzymać ten błąd, jeśli wiadomości są routowane przez 3 usługa firmy. Można użyć narzędzia wyszukiwania WHOIS odnaleźć właściciela zablokowanych adresów IP.
    


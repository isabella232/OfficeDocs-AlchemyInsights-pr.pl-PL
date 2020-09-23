---
title: 726 blokowanie przekierowywania poczty e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219865"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokowanie i odblokowywanie przekierowywania poczty e-mail

Aby włączyć lub wyłączyć przesyłanie dalej wiadomości e-mail dla konkretnej skrzynki pocztowej, zobacz [Konfigurowanie przekierowywania poczty e-mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Po przeprowadzeniu kontroli nad przekazaniem zewnętrznym na poziomie dzierżawy jest używana zasada zapobiegania spamowi. Jeśli to ustawienie jest wyłączone lub automatyczne, możesz zablokować przesyłanie poczty e-mail przy użyciu funkcji "550 5.7.520 Access odmowa dostępu, ponieważ organizacja nie zezwala na błąd w Twojej zewnętrznej przekierowaniu". Następnie, jeśli przesyłanie dalej zostało ustawione jako zablokowane, to jest błąd widoczny dla użytkowników.

Jeśli przesyłanie dalej jest blokowane, upewnij się, że skonfigurowano zasady umożliwiające włączenie zewnętrznego autoprzekazywania. Zasady filtrowania z wychodzącymi spamami można sprawdzić w centrum zabezpieczeń i zgodności albo przez uruchomienie polecenia Get-HostedOutboundSpamFilterPolicy | Nazwa FL, autoprzesyłanie dalej. Jeśli chcesz skonfigurować blokowanie autoprzesyłania dalej, to samo polecenie poinformuje Cię o stanie zasad teraz.

Uwaga: zaleca się pozostawienie zewnętrznego autowiadomości bez wyłączenia na domyślnych zasadach filtrowania spamu dla połączeń wychodzących i włączenie tej funkcji tylko dla użytkowników wymagających przekierowania zewnętrznego przez utworzenie dla tych użytkowników zasad niestandardowych. Aby dowiedzieć się więcej, zobacz [Konfigurowanie zewnętrznej obsługi przekierowywania wiadomości e-mail w pakiecie Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
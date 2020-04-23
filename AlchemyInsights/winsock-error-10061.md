---
title: 1554 Błąd Winsocka 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766179"
---
# <a name="winsock-error-10061"></a>Błąd Winsocka 10061

Ten kod błędu oznacza, że firma Microsoft nie może ustanowić gniazda TCP (połączenia) z hostem docelowym. Najbardziej prawdopodobną przyczyną tego błędu jest problem z konfiguracją zapory. Aby rozwiązać ten problem, sprawdź następujące ustawienia:

- Weryfikowanie konfiguracji zapory za pomocą informacji w [adresach URL i zakresach adresów IP usługi Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Jeśli błąd dotyczy programu Exchange Online Protection (EOP), użytkownik powinien zostać wcześniej powiadomiony o zmianie [adresów IP ochrony usługi Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)Protection .

- Sprawdź, czy usługodawca internetowy nie blokuje portu.

- Sprawdź ustawienia hosta inteligentnego i serwera docelowego w łącznikach.

Należy zauważyć, że usługa Microsoft 365 nie blokuje połączeń *przychodzących* w ten sposób.

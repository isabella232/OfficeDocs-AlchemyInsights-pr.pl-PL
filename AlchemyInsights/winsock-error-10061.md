---
title: '1554: błąd Winsock 10061'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083240"
---
# <a name="winsock-error-10061"></a>Błąd Winsocka 10061

Ten kod błędu oznacza, że firma Microsoft nie mogła nawiązać połączenia (socket) TCP z hostem docelowym. Najprawdopodobniej przyczyną tego błędu jest problem z konfiguracją zapory. Aby rozwiązać ten problem, sprawdź następujące ustawienia:

- Sprawdzanie konfiguracji zapory przy użyciu informacji z Microsoft 365 URL i [zakresów](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) adresów IP

- Jeśli błąd dotyczy konkretnej Exchange Online Protection (EOP), należy wcześniej został powiadomiony o zmianie adresu IP usługi [Exchange Online Protection IP.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Sprawdź, czy usługodawca internetowy (ISP) nie blokuje portu.

- Sprawdź ustawienia hosta inteligentnego i serwera docelowego w łącznikach.

Pamiętaj, Microsoft 365 nie blokuje połączeń *przychodzących* w ten sposób.

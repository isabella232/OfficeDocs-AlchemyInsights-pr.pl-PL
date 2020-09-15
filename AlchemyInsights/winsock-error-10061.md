---
title: 1554 błąd Winsock 10061
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698872"
---
# <a name="winsock-error-10061"></a>Błąd Winsock 10061

Ten kod błędu oznacza, że firma Microsoft nie mogła ustanowić gniazda TCP (połączenia) z hostem docelowym. Najbardziej prawdopodobną przyczyną tego błędu jest problem z konfiguracją zapory. Aby rozwiązać ten problem, sprawdź następujące ustawienia:

- Weryfikowanie konfiguracji zapory przy użyciu informacji z [adresów URL i zakresów adresów IP programu Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Jeśli błąd jest specyficzny dla usługi Exchange Online Protection (EOP), należy wcześniej powiadomić o zmianach [adresów IP usługi Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Sprawdź, czy Twój dostawca usług internetowych (ISP) nie blokuje portu.

- Sprawdź ustawienia hosta inteligentnego i serwera docelowego w łącznikach.

Pamiętaj, że program Microsoft 365 nie blokuje połączeń *przychodzących* w ten sposób.

---
title: Błąd warstwy Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 3fa3b2f2e10d3ebe480861e1f2d7ecaa262afe14
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757112"
---
# <a name="winsock-error-10061"></a>Błąd warstwy Winsock 10061

Ten kod błędu oznacza, że usługi Office 365, nie można ustanowić gniazda TCP (połączenie) z hosta docelowego. Najbardziej prawdopodobną przyczyną tego błędu jest problem z konfiguracją zapory. Aby rozwiązać ten problem, sprawdź następujące ustawienia:

- Sprawdź konfigurację zapory przy użyciu informacji z [zakresów adresów IP i adresy URL usługi Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Jeśli błąd jest specyficzny na Exchange Online ochrony (podniesienie uprawnień), możesz powinny zostały wcześniej zgłoszone do zmiany na [adresy IP ochrony Online programu Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Sprawdź, czy usługodawcy internetowego (ISP) nie blokuje port.

- Sprawdź inteligentne ustawienia serwera hosta i docelowego w złącza.

Należy zauważyć, że usługi Office 365 nie blokuje połączenia *przychodzące* w ten sposób.

---
title: Naprawianie reguł transportu
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034764"
---
# <a name="fix-transport-rules"></a>Naprawianie reguł transportu

Ta wiadomość została wpłynęła na niestandardową regułę przepływu poczty e-mail. Aby sprawdzić dokładną regułę, wykonaj następujące czynności:

1. W wynikach przesyłania w **obszarze Informacje dodatkowe** zanotuj identyfikator **GUID** lub **nazwę zasad.**
2. Uruchom Exchange zarządzania. Aby uzyskać więcej informacji, [zobacz Otwieranie Exchange zarządzania danymi.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Uruchom to polecenie (przy użyciu identyfikatora GUID z Twojego przesłania):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Przejrzyj opis, aby zobaczyć skonfigurowane warunki, które wpłynęły na wiadomość.

Aby dowiedzieć się więcej, [zobacz Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)

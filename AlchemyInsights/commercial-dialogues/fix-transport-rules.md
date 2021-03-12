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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750579"
---
# <a name="fix-transport-rules"></a>Naprawianie reguł transportu

Ta wiadomość została wpłynęła na niestandardową regułę przepływu poczty e-mail. Aby sprawdzić dokładną regułę, wykonaj następujące czynności:

1. W wynikach przesyłania w **obszarze Informacje dodatkowe** zanotuj identyfikator **GUID** lub **nazwę zasad.**
2. Uruchom powłokę zarządzania programu Exchange. Aby uzyskać więcej informacji, [zobacz Otwieranie powłoki zarządzania programu Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Uruchom to polecenie (przy użyciu identyfikatora GUID z Twojego przesłania):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Przejrzyj opis, aby zobaczyć skonfigurowane warunki, które wpłynęły na wiadomość.

Aby dowiedzieć się więcej, [zobacz Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)

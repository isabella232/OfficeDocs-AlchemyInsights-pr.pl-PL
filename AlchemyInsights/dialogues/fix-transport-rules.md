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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695857"
---
# <a name="fix-transport-rules"></a>Naprawianie reguł transportu

Wiadomość wpłynęła na niestandardową regułę przepływu poczty e-mail. Aby zapoznać się z dokładną regułą, wykonaj następujące czynności:

1. W wynikach przesyłania w obszarze **Informacje dodatkowe** zwróć uwagę na identyfikator **GUID** lub **nazwę zasad.**
2. Uruchom powłokę zarządzania programem Exchange. Aby uzyskać więcej informacji, [zobacz Otwieranie powłoki zarządzania programem Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Uruchom to polecenie (używając identyfikatora GUID z Twojego przesłania):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Przejrzyj opis, aby zobaczyć skonfigurowane warunki, które wpłynęły na wiadomość.

Aby dowiedzieć się więcej, [zobacz Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)

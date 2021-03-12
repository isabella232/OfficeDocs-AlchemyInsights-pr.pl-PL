---
title: Naprawianie zasad dzierżawy (zastępowanie akcji)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748993"
---
# <a name="fix-tenant-policy-action-override"></a>Naprawianie zasad dzierżawy (zastępowanie akcji)

Ta wiadomość została podysłana przez zasady ochrony przed spamem w dzierżawie. Aby przejrzeć zasady, wykonaj następujące czynności:

1. Przejdź do Centrum zabezpieczeń [usługi Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143) zgodności , a następnie przejdź do strony Ochrona przed spamem przy zasadach zarządzania  >    >  [zagrożeniami.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Sprawdź, czy  źródło zasad wskazuje następujące informacje: **Komunikat Add-Xheader/ModifySubject/Redirect/Delete/No action/ UDW**

    Jeśli tak, na **karcie Niestandardowy** sprawdź ustawienia zasad, których dotyczyła wiadomość. Możliwe, że wiadomość  wpłynęła na ustawienia standardowe zastosowane do wszystkich klientów usługi Exchange Online Protection.

Aby uzyskać więcej informacji na temat konfigurowania zasad filtrowania spamu, zobacz [Konfigurowanie zasad filtru spamu.](https://go.microsoft.com/fwlink/?linkid=2101431)

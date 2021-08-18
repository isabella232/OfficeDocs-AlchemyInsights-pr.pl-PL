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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326807"
---
# <a name="fix-tenant-policy-action-override"></a>Naprawianie zasad dzierżawy (zastępowanie akcji)

Jedna z zasad ochrony przed spamem wpłynęła na tę wiadomość. Aby przejrzeć zasady, wykonaj następujące czynności:

1. W portalu Microsoft 365 Defender pod adresem przejdź do sekcji & e-mail i zasad współpracy & zasady zagrożeń zapobiegające <https://security.microsoft.com/>  \>  \>  \> **spamowi.** 

   Aby przejść bezpośrednio do strony Zasady ochrony **przed spamem,** <https://security.microsoft.com/antispam> użyj .

2. Na stronie Zasady ochrony przed **spamem** wybierz zasady, klikając nazwę zasad **(** Wpisz  Niestandardowa zasada ochrony przed spamem lub Nazwa to Zasady przychodzące ochrony przed **spamem** **(domyślnie)**).
3. W wyświetlonym wysuwanych szczegółach wybierz **pozycję Edytuj akcje** w **sekcji** Akcje.
4. W sekcji Akcje **wiadomości** przejrzyj werdykty dotyczące spamu,  spamu o dużej **pewności,** wyłudzania informacji i wyłudzania informacji o wysokiej pewności, aby sprawdzić, czy jest zaznaczona dowolna z następujących wartości:
   - **Dodawanie nagłówka X-header**
   - **Przed wierszem tematu tekstem**
   - **Przekierowywanie wiadomości na adres e-mail**
   - **Usuwanie wiadomości**
   - **Brak akcji**

   Możliwe, że ustawienia **Standardowe zastosowane** do wszystkich Exchange Online Protection wpłynęły na wiadomość.

Aby uzyskać więcej informacji, [zobacz Konfigurowanie zasad ochrony przed spamem w u usługi EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)

---
title: Naprawianie zasad połączenia
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314854"
---
# <a name="fix-connection-policy"></a>Naprawianie zasad połączenia

Wiadomość e-mail została oznaczona jako bezpieczna i dostarczona do Skrzynki odbiorczej użytkownika, ponieważ źródłowy adres IP został oznaczony jako bezpieczny w domyślnych zasadach filtru połączenia. Aby przejrzeć zasady, wykonaj następujące czynności:

1. W portalu Microsoft 365 Defender pod adresem przejdź do sekcji & e-mail i zasad współpracy & zasady zagrożeń zapobiegające <https://security.microsoft.com/>  \>  \>  \> **spamowi.** 

   Aby przejść bezpośrednio do strony Zasady ochrony **przed spamem,** <https://security.microsoft.com/antispam> użyj .

2. Na stronie **Zasady ochrony przed spamem** wybierz zasady o nazwie Zasady filtru połączenia **(domyślne),** klikając nazwę zasad.

3. W wyświetlonym wysuwaniu szczegółów kliknij pozycję **Edytuj zasady filtru połączenia** w sekcji **Filtrowanie** połączenia.

4. Przejrzyj wpisy w sekcji Zawsze pozwalaj na wiadomości z następujących adresów IP lub z zakresu adresów **i** sprawdź, czy jest **zaznaczona** opcja Włącz listę bezpiecznych adresów.

   **Uwaga:** Firma Microsoft subskrybuje zewnętrzne źródła zaufanych nadawców. Jeśli lista bezpiecznych adresów jest włączona, zaufani nadawcy nie są omyłowo oznaczani jako spam. Zalecamy zaznaczenie tej opcji, ponieważ spowoduje to zmniejszenie liczby odbieranych wyników fałszywie dodatnich (oznaczanych dobrą wiadomością, która jest klasyfikowana jako spam).

Aby uzyskać więcej informacji, [zobacz Konfigurowanie filtrowania połączeń.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)

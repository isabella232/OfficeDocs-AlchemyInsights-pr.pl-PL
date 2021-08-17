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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888416"
---
# <a name="fix-connection-policy"></a>Naprawianie zasad połączenia

Wiadomość e-mail została oznaczona jako bezpieczna i dostarczona do Skrzynki odbiorczej użytkownika, ponieważ źródłowy adres IP został oznaczony jako bezpieczny w domyślnych zasadach filtru połączenia. Aby przejrzeć zasady, wykonaj następujące czynności:

1. W portalu Microsoft 365 Defender pod adresem przejdź do sekcji Zasady & e-mail & zasady zagrożeń zapobiegające <https://security.microsoft.com/>  \>  \>  \> **spamowi.** 

   Aby przejść bezpośrednio do strony Zasady ochrony **przed spamem,** <https://security.microsoft.com/antispam> użyj .

2. Na stronie **Zasady ochrony przed spamem** wybierz zasady o nazwie Zasady filtru połączenia **(domyślne),** klikając nazwę zasad.

3. W wyświetlonym wysuwaniu szczegółów kliknij pozycję **Edytuj zasady filtru połączenia** w sekcji **Filtrowanie** połączenia.

4. Przejrzyj wpisy w sekcji Zawsze pozwalaj na wiadomości z następujących adresów IP lub z zakresu adresów **i** sprawdź, czy jest **zaznaczona** opcja Włącz listę bezpiecznych adresów.

   > [!NOTE]
   > Firma Microsoft subskrybuje zewnętrzne źródła zaufanych nadawców. Jeśli lista bezpiecznych adresów jest włączona, zaufani nadawcy nie są omyłowo oznaczani jako spam. Zalecamy zaznaczenie tej opcji, ponieważ spowoduje to zmniejszenie liczby odbieranych wyników fałszywie dodatnich (oznaczanych dobrą wiadomością, która jest klasyfikowana jako spam).

Aby uzyskać więcej informacji, [zobacz Konfigurowanie filtrowania połączeń.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)

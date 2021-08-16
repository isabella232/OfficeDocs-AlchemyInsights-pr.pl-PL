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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988131"
---
# <a name="fix-connection-policy"></a>Naprawianie zasad połączenia

Wiadomość e-mail została oznaczona jako bezpieczna i dostarczona do skrzynki odbiorczej użytkownika, ponieważ wysyłający adres IP został oznaczony jako bezpieczny w zasadach Filtr połączenia. Aby przejrzeć zasady, wykonaj następujące czynności:

1. Przejdź do Centrum [Office 365 zabezpieczeń &](https://go.microsoft.com/fwlink/p/?linkid=2077143), a następnie przejdź do strony Ochrona przed spamem przy zasadach zarządzania  >    >  [zagrożeniami.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Na karcie **Niestandardowe** wybierz zasady **filtru połączenia**, a następnie wybierz pozycję **Edytuj zasady**.
3. Przejrzyj listę **adresów IP Allow (Zezwalaj).** Sprawdź, **Sejf jest** włączona.

    > [!NOTE]
    > Firma Microsoft subskrybuje zewnętrzne źródła zaufanych nadawców. Jeśli **Sejf jest włączona,** oznacza to, że ci zaufani nadawcy nie są omyłowo oznaczani jako spam. Zalecam zaznaczenie tej opcji, ponieważ spowoduje to zmniejszenie liczby odbieranych wyników fałszywie dodatnich (good mail, które są klasyfikowane jako spam).

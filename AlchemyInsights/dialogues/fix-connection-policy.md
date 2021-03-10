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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695883"
---
# <a name="fix-connection-policy"></a>Naprawianie zasad połączenia

Wiadomość e-mail została oznaczona jako bezpieczna i dostarczona do skrzynki odbiorczej użytkownika, ponieważ wysyłający adres IP został oznaczony jako bezpieczny w zasadach filtru połączenia. Aby przejrzeć zasady, wykonaj następujące czynności:

1. Przejdź do Centrum zabezpieczeń usługi [Office 365 & zgodności,](https://go.microsoft.com/fwlink/p/?linkid=2077143)a następnie przejdź do strony Ochrona przed spamem w zasadach zarządzania   >    >  [zagrożeniami.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Na karcie **Niestandardowe** wybierz **zasady** filtrowania połączenia, a następnie wybierz pozycję **Edytuj zasady.**
3. Przejrzyj listę **ze zezwalaniem na adresy IP.** Sprawdź, **czy jest włączona lista** bezpiecznych adresów.

    > [!NOTE]
    > Firma Microsoft subskrybuje zewnętrzne źródła zaufanych nadawców. Jeśli **jest włączona** bezpieczna lista, zaufani nadawcy nie są oznaczani przez pomyłkę jako spam. Zalecam zaznaczenie tej opcji, ponieważ spowoduje to zmniejszenie liczby odbieranych wyników fałszywie dodatnich (dobrej poczty klasyfikowanej jako spam).

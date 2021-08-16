---
title: błąd Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049318"
---
# <a name="4c7-error-in-microsoft-teams"></a>Błąd 4c7 w Microsoft Teams

Ten błąd występuje, ponieważ Microsoft Teams uwierzytelniania formularzy. Po wdrożeniu usług feder formowych Active Directory (AD FS) uwierzytelnianie formularzy nie jest domyślnie włączone w intranecie. Jeśli Windows zintegrowane uwierzytelnianie nie powiedzie się, zostanie wyświetlony monit o zalogowanie się przy użyciu uwierzytelniania formularzy.

Aby rozwiązać ten problem, włącz uwierzytelnianie formularzy przy użyciu Microsoft Management Console AD FS (MMC) na komputerze, na którym znajduje się kopia lokalna usługi Active Directory. Aby to zrobić, wykonaj następujące kroki. 

1. W okienku nawigacji przejdź do strony **Zasady uwierzytelniania.**
2. W **obszarze Akcje** w okienku szczegółów wybierz pozycję Edytuj globalne **uwierzytelnianie podstawowe**.
3. Na karcie **Intranet** wybierz pozycję **Uwierzytelnianie formularzy**.
4. Wybierz **przycisk OK** (lub **Zastosuj).**
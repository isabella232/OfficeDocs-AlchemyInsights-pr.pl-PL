---
title: Błąd teams 4c7
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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786679"
---
# <a name="4c7-error-in-microsoft-teams"></a>Błąd 4c7 w aplikacji Microsoft Teams

Ten błąd występuje, ponieważ aplikacja Microsoft Teams wymaga uwierzytelniania formularzy. Po wdrożeniu usług feder formowych Active Directory (AD FS) uwierzytelnianie formularzy nie jest domyślnie włączone w intranecie. Jeśli zintegrowane uwierzytelnianie systemu Windows nie powiedzie się, zostanie wyświetlony monit o zalogowanie się przy użyciu uwierzytelniania formularzy.

Aby rozwiązać ten problem, włącz uwierzytelnianie formularzy przy użyciu Microsoft Management Console AD FS (MMC) na komputerze, na którym znajduje się kopia lokalna usługi Active Directory. Aby to zrobić, wykonaj następujące kroki. 

1. W okienku nawigacji przejdź do strony **Zasady uwierzytelniania.**
2. W **obszarze Akcje** w okienku szczegółów wybierz pozycję Edytuj globalne **uwierzytelnianie podstawowe**.
3. Na karcie **Intranet** wybierz pozycję **Uwierzytelnianie formularzy**.
4. Wybierz **przycisk OK** (lub **Zastosuj).**
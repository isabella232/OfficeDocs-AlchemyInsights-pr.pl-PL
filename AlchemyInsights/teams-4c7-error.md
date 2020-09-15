---
title: Błąd 4c7 aplikacji Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700213"
---
# <a name="4c7-error-in-microsoft-teams"></a>błąd 4c7 w aplikacji Microsoft Teams

Ten błąd występuje, ponieważ aplikacja Microsoft Teams wymaga uwierzytelniania formularzy. Podczas wdrażania usług federacyjnych Active Directory (AD FS) uwierzytelnianie formularzy nie jest domyślnie włączone dla intranetu. Jeśli zintegrowane uwierzytelnianie systemu Windows nie powiedzie się, zostanie wyświetlony monit o zalogowanie się przy użyciu uwierzytelniania formularzy.

Aby rozwiązać ten problem, Włącz uwierzytelnianie formularzy za pomocą przystawki Microsoft Management Console (MMC) programu AD FS na komputerze, na którym jest używana kopia lokalna usługi Active Directory. Aby to zrobić, wykonaj następujące kroki. 

1. W okienku nawigacji przejdź do **zasad uwierzytelniania**.
2. W obszarze **Akcje** w okienku szczegółów wybierz pozycję **Edytuj globalne uwierzytelnianie podstawowe**.
3. Na karcie **intranet** wybierz pozycję **uwierzytelnianie formularzy**.
4. Wybierz **przycisk OK** (lub **Zastosuj**).
---
title: Drużyny 4c7 błąd
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796280"
---
# <a name="4c7-error-in-microsoft-teams"></a>błąd 4c7 w programie Microsoft Teams

Ten błąd występuje, ponieważ Microsoft Teams wymaga uwierzytelniania formularzy. Podczas wdrażania programu Active Directory Federation Services (AD FS), uwierzytelnianie formularzy nie jest włączona dla intranetu domyślnie. Jeśli zintegrowane uwierzytelnianie systemu Windows nie powiedzie się, zostanie wyświetlony monit o zalogowanie się przy użyciu uwierzytelniania formularzy.

Aby rozwiązać ten problem, należy włączyć uwierzytelnianie formularzy przy użyciu przystawki programu AD FS Microsoft Management Console (MMC) na komputerze, który ma lokalną kopię usługi Active Directory. W tym celu wykonaj następujące czynności: 

1. W okienku nawigacji przejdź do **zasad uwierzytelniania**.
2. W obszarze **Akcje** w okienku szczegółów wybierz opcję **Edytuj globalne uwierzytelnianie podstawowe**.
3. Na karcie **intranet** wybierz opcję **uwierzytelnianie formularzy**.
4. Wybierz **OK** (lub **Zastosuj**).
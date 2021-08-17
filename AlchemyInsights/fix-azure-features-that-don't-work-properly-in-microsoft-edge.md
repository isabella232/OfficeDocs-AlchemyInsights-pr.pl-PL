---
title: Co zrobić, jeśli funkcje platformy Azure nie działają poprawnie w Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117098"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Co zrobić, jeśli funkcje platformy Azure nie działają poprawnie w Microsoft Edge

Microsoft Edge mają [znane problemy związane](https://go.microsoft.com/fwlink/?linkid=2140608) ze strefami zabezpieczeń i mogą mieć wpływ na sposób logowania się użytkowników platformy Azure do Windows administracyjnego. Jeśli masz problem z używaniem funkcji platformy Azure z usługą Microsoft Edge, spróbuj wykonać następujące czynności:

1. W menu **Start** wyszukaj polecenie **Opcje internetowe** i wybierz je.
2. W **oknie dialogowym** Właściwości internetowe przejdź do **karty Zabezpieczenia.**
3. Wybierz **strefę Zaufane witryny,** a następnie wybierz **przycisk** Witryny.
4. W **oknie dialogowym Zaufane** witryny dodaj adres URL bramy oraz pozycję , a [https://login.microsoftonline.com](https://login.microsoftonline.com) następnie wybierz pozycję [https://login.live.com](https://login.live.com) **Zamknij**.
5. W **oknie dialogowym** Właściwości internetowe przejdź do **karty Prywatność.**
6. W sekcji **Blokowanie wyskakujących okienek** wybierz pozycję **Ustawienia**. W oknie dialogowym, które zostanie otwarte, dodaj adres URL bramy oraz pozycję , a [https://login.microsoftonline.com](https://login.microsoftonline.com) następnie wybierz pozycję [https://login.live.com](https://login.live.com) **Zamknij**.

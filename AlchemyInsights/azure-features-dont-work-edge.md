---
title: Co zrobić, jeśli funkcje platformy Azure nie działają poprawnie w Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812874"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Co zrobić, jeśli funkcje platformy Azure nie działają poprawnie w Microsoft Edge

Microsoft Edge mają znane problemy związane ze strefami zabezpieczeń, które mogą mieć wpływ na sposób logowania się użytkowników platformy Azure Windows centrum administracyjnym. Aby uzyskać więcej informacji, zobacz [Znane problemy dotyczące edge.](https://go.microsoft.com/fwlink/?linkid=2140608) Jeśli masz problem z używaniem funkcji platformy Azure z usługą Microsoft Edge, spróbuj wykonać następujące czynności:

1. Na pasku menu Start wpisz opcje  internetowe **,** a następnie wybierz tę pozycję.
1. W **oknie Właściwości** internetowe wybierz **kartę** Zabezpieczenia.
1. Wybierz **pozycję Zaufane witryny**, a następnie wybierz pozycję **Witryny**.
1. Dodaj adres URL bramy, a także <https://login.microsoftonline.com> i , a następnie wybierz pozycję <https://login.live.com> **Zamknij**.
1. W **oknie Właściwości** internetowe wybierz **kartę** Prywatność.
1. W sekcji Blokowanie wyskakujących okienek wybierz pozycję **Ustawienia**. Dodaj adres URL bramy, a także <https://login.microsoftonline.com> i , a następnie wybierz pozycję <https://login.live.com> **Zamknij**.
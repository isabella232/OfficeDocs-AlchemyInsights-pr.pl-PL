---
title: Co zrobić, jeśli funkcje platformy Azure nie działają poprawnie w programie Microsoft Edge
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
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583787"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Co zrobić, jeśli funkcje platformy Azure nie działają poprawnie w programie Microsoft Edge

W programie Microsoft Edge występują [znane problemy](https://go.microsoft.com/fwlink/?linkid=2140608) dotyczące stref zabezpieczeń, które mogą wpływać na sposób logowania użytkowników platformy Azure do centrum administracyjnego systemu Windows. Jeśli masz problemy z korzystaniem z funkcji platformy Azure w programie Microsoft Edge, spróbuj wykonać następujące czynności:

1. W menu **Start** Wyszukaj polecenie **Opcje internetowe** i wybierz je.
2. W oknie dialogowym **Właściwości internetowe** przejdź do karty **zabezpieczenia** .
3. Wybierz strefę **Zaufane witryny** , a następnie wybierz przycisk **witryny** .
4. W oknie dialogowym **Zaufane witryny** Dodaj adres URL bramy oraz [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) pozycję, a następnie wybierz pozycję **Zamknij**.
5. W oknie dialogowym **Właściwości internetowe** przejdź do karty **prywatność** .
6. W sekcji **Blokowanie wyskakiwania okien** wybierz pozycję **Ustawienia**. W otwartym oknie dialogowym Dodaj adres URL bramy oraz [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) pozycję, a następnie wybierz pozycję **Zamknij**.

---
title: 0x8004de40 błąd podczas uruchamiania usługi OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823113"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 błąd podczas uruchamiania usługi OneDrive

Jeśli podczas logowania do usługi OneDrive zostanie wyświetlony komunikat o błędzie **0x8004de40** , uruchom ponownie komputer po połączeniu z domeną służbową lub szkolną. Jeśli po ponownym uruchomieniu komputera pojawi się ten błąd, spróbuj wykonać tę czynność po połączeniu z domeną służbową lub szkolną:

1. Kliknij przycisk Start, a następnie wpisz ciąg **cmd** lub **Command**  w polu wyszukiwania, kliknij prawym przyciskiem myszy aplikację wiersza polecenia, a następnie wybierz pozycję  **Uruchom jako administrator** . Jeśli zostanie wyświetlony monit o podanie hasła administratora lub potwierdzenie, wpisz hasło lub kliknij pozycję **Zezwalaj** .  

2. W oknie wiersza polecenia wpisz **dsregcmd/Leave**  i poczekaj na ukończenie polecenia. Następnie wpisz **dsregcmd/Join** i poczekaj na ukończenie polecenia.
3. Uruchom ponownie komputer.

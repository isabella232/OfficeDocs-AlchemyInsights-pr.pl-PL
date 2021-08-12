---
title: 0x8004de40 błędu podczas uruchamiania OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946589"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 błędu podczas uruchamiania OneDrive

Jeśli podczas logowania się do usługi **0x8004de40** do usługi OneDrive zostanie wyświetlony komunikat o błędzie, uruchom ponownie komputer, gdy jest połączony z domeną służbowej lub szkolnej. Jeśli po ponownym uruchomieniu komputera zostanie wyświetlony ten błąd, spróbuj wykonać tę próbę, gdy komputer jest połączony z domeną służbowej lub szkolnej:

1. Kliknij przycisk Start i wpisz **cmd** lub **wiersz** polecenia w polu wyszukiwania, kliknij prawym przyciskiem myszy aplikację wiersza polecenia i wybierz **pozycję Uruchom jako administrator.** Jeśli zostanie wyświetlony monit o hasło administratora lub potwierdzenie, wpisz hasło lub kliknij przycisk **Zezwalaj**.  

2. W oknie Wiersz polecenia wpisz **dsregcmd /leave**  i poczekaj na ukończenie polecenia. Następnie wpisz **dsregcmd /join** i poczekaj na ukończenie polecenia.
3. Uruchom ponownie komputer.

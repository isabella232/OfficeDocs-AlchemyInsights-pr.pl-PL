---
title: błąd 0x8004de40 podczas uruchamiania usługi OneDrive
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
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813662"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>błąd 0x8004de40 podczas uruchamiania usługi OneDrive

Jeśli podczas logowania się **do usługi** OneDrive 0x8004de40 komunikat o błędzie, uruchom ponownie komputer, gdy komputer jest połączony z domeną służbowej lub szkolnej. Jeśli po ponownym uruchomieniu komputera zostanie wyświetlony ten błąd, spróbuj wykonać tę próbę, gdy komputer jest połączony z domeną służbowej lub szkolnej:

1. Kliknij przycisk Start i wpisz **cmd** lub **wiersz** polecenia w polu wyszukiwania, kliknij prawym przyciskiem myszy aplikację wiersza polecenia i wybierz **pozycję Uruchom jako administrator.** Jeśli zostanie wyświetlony monit o hasło administratora lub potwierdzenie, wpisz hasło lub kliknij przycisk **Zezwalaj**.  

2. W oknie Wiersz polecenia wpisz **dsregcmd /leave**  i poczekaj na ukończenie polecenia. Następnie wpisz **dsregcmd /join** i poczekaj na ukończenie polecenia.
3. Uruchom ponownie komputer.

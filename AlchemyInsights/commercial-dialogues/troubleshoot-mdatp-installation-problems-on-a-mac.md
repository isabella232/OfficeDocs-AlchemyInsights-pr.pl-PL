---
title: Rozwiązywanie problemów z instalacją MDATP na komputerze Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749773"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Rozwiązywanie problemów z instalacją MDATP na komputerze Mac

Jeśli instalacja ręczna nie powiedzie się, **na stronie Podsumowanie** kreatora instalacji jest wyświetlany następujący błąd:

"Wystąpił błąd podczas instalacji. Instalator napotkał błąd, który powodował niepowodzenie instalacji. Aby uzyskać pomoc, skontaktuj się z producentem oprogramowania".

W przypadku wdrożeń MDM na stronie przedstawiono również ogólny błąd instalacji.

Chociaż użytkownicy końcowi nie wyświetlają dokładnych błędów, plik dziennika jest w toku instalacji, w **/Library/Logs/Microsoft/mdatp/install.log.** Każda sesja instalacji jest dołączana do tego pliku dziennika. Aby wy wyprowadzić tylko ostatnią sesję instalacji, użyj `sed` .

Aby dowiedzieć się więcej, zobacz Rozwiązywanie problemów z instalacją [programu Microsoft Defender ATP dla komputerów Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)

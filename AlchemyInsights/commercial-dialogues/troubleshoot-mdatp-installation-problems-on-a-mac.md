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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091061"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Rozwiązywanie problemów z instalacją MDATP na komputerze Mac

Jeśli instalacja ręczna nie powiedzie się, **na stronie Podsumowanie** kreatora instalacji jest wyświetlany następujący błąd:

"Wystąpił błąd podczas instalacji. Instalator napotkał błąd, który powodował niepowodzenie instalacji. Aby uzyskać pomoc, skontaktuj się z producentem oprogramowania".

W przypadku wdrożeń MDM na stronie przedstawiono również ogólny błąd instalacji.

Chociaż użytkownicy końcowi nie wyświetlają dokładnych błędów, plik dziennika jest w toku instalacji, w **/Library/Logs/Microsoft/mdatp/install.log.** Każda sesja instalacji jest dołączana do tego pliku dziennika. Aby wy wyprowadzić tylko ostatnią sesję instalacji, użyj `sed` .

Aby dowiedzieć się więcej, zobacz Rozwiązywanie problemów z instalacją [programu Microsoft Defender ATP dla komputerów Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)

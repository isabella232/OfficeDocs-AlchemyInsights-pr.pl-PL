---
title: Problemy z instalowaniem programu Microsoft Defender na komputerach Mac lub Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 6646ca4792ac4d9fb8bfb7433d53ecf4aeba8da0aca797225c16c02b28499889
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013254"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemy z instalowaniem programu Microsoft Defender na komputerach Mac lub Linux

**Mac**

- Przed zainstalowaniem programu Microsoft Defender ATP dla komputerów Mac upewnij się, że są spełnione wymagania systemowe. Aby uzyskać więcej informacji, zobacz [Jak zainstalować program Microsoft Defender ATP dla komputerów Mac.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Przejrzyj informacje w pliku: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Przed zainstalowaniem programu Microsoft Defender ATP dla systemu Linux upewnij się, że są spełnione wymagania systemowe. Aby uzyskać więcej informacji, zobacz [Jak zainstalować usługę MDATP dla systemu Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Aby sprawdzić, czy usługa MDATP jest uruchomiona, zobacz [Instalacja nie powiodła się.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Aby rozwiązać problemy, jeśli usługa nie jest uruchomiona, zobacz Kroki rozwiązywania problemów z nieuprawnianą usługą [MDATP.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Instrukcje sprawdzania konfiguracji klienta, która pozwala na sprawdzenie kondycji produktu, oraz uruchomienia testu wykrywania w pliku tekstowym EICAR, zawiera [temat Konfiguracja klienta.](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Uwaga** Aby uzyskać listę obsługiwanych systemów plików dla działań przy dostępie, zobacz [Microsoft Defender ATP for Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)
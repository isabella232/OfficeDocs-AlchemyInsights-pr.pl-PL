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
ms.openlocfilehash: defc11265caf371ce0a62a10a5de1d8ff88a8e11
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325259"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemy z instalowaniem programu Microsoft Defender na komputerach Mac lub Linux

**Mac**

- Przed zainstalowaniem programu Microsoft Defender ATP dla komputerów Mac upewnij się, że są spełnione wymagania systemowe. Aby uzyskać więcej informacji, zobacz [Jak zainstalować program Microsoft Defender ATP dla komputerów Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Przejrzyj informacje w pliku: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Przed zainstalowaniem programu Microsoft Defender ATP dla systemu Linux upewnij się, że są spełnione wymagania systemowe. Aby uzyskać więcej informacji, zobacz [Jak zainstalować usługę MDATP dla systemu Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- Aby sprawdzić, czy usługa MDATP jest uruchomiona, zobacz [Instalacja nie powiodła się.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Aby rozwiązać problemy, jeśli usługa nie jest uruchomiona, zobacz Kroki rozwiązywania problemów z nieuprawnianą usługą [MDATP.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- Aby uzyskać instrukcje sprawdzania konfiguracji klienta, która sprawdza kondycję produktu, oraz uruchomienia testu wykrywania w pliku tekstowym EICAR, zobacz [Konfiguracja klienta.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **Uwaga** Aby uzyskać listę obsługiwanych systemów plików dla działań przy dostępie, zobacz [Microsoft Defender ATP for Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)
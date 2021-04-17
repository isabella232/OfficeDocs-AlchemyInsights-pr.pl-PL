---
title: Zainstalowano aplikację Teams z aktualizacjami pakietu Office
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
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: 36b0b1a7bf37c27304b4124157dba9aba337678c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832392"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Aplikacja Microsoft Teams zainstalowana z aktualizacjami pakietu Office

Aplikacja Microsoft Teams jest  dołączona do nowych instalacji aplikacji Platformy Microsoft 365 dla przedsiębiorstw, aplikacji platformy Microsoft 365 dla firm i pakietu Office dla komputerów Mac. Aby uzyskać więcej informacji, zobacz Kiedy usługa Microsoft Teams zacznie być [dołączona do nowych instalacji pakietu Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ponadto, począwszy od wersji 1906 w bieżącym kanale,  zespoły będą stopniowo dodawane do istniejących instalacji aplikacji Microsoft 365 dla przedsiębiorstw (i Aplikacji Microsoft 365 dla firm) na urządzeniach z systemem Windows po zaktualizowaniu istniejącej instalacji do najnowszej wersji. Aby uzyskać więcej informacji, zobacz [Co z istniejącymi instalacjami pakietu Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Uwaga:** Jeśli nie chcesz czekać na ten harmonogram wdrożenia, możesz wdrożyć aplikację Teams jako autonomiczną dla swoich użytkowników, korzystając z tych instrukcji [lub](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)zainstalować aplikację Teams dla siebie z https://teams.microsoft.com/downloads .

Jeśli Twoja organizacja nie jest jeszcze gotowa do wdrożenia usługi Teams, możesz wykluczyć aplikację ***Teams*** z [nowych](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) lub istniejących [instalacji](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) pakietu Office. Jeśli chcesz, aby aplikacja Teams była instalowana, ale nie chcesz, aby aplikacja Teams uruchamiała się automatycznie dla użytkownika po jej zainstalowaniu, zobacz Uniemożliwianie automatycznego uruchamiania aplikacji Microsoft Teams po [zakończeniu instalacji.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Aby ***odinstalować aplikację Teams*** z urządzenia z systemem Windows, zobacz [Odinstalowywanie aplikacji Microsoft Teams.](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81) Aby oczyścić usługę Microsoft Teams z wielu komputerów docelowych lub użytkowników, zobacz [Oczyszczanie wdrożenia usługi Microsoft Teams.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Jeśli korzystasz z komputerów udostępnionych, usług pulpitu zdalnego (RDS) lub infrastruktury pulpitów wirtualnych (VDI), zobacz Środowisko komputerów udostępnionych i [środowisk VDI](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)w aplikacji Microsoft Teams. Jeśli korzystasz z pakietu Office dla komputerów Mac, zobacz Instalacje [aplikacji Microsoft Teams na komputerze Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Uwaga:** Po zainstalowaniu aplikacji Teams jest ona automatycznie [aktualizowana](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) co około dwa tygodnie o nowe funkcje i aktualizacje jakości. 
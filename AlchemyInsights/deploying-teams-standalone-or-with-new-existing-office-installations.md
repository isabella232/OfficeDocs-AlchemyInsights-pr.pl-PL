---
title: Wdrażanie Teams jako autonomicznego lub z nowymi lub istniejącymi Office instalacjami
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320132"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Wdrażanie Teams jako autonomicznego lub z nowymi lub istniejącymi Office instalacjami

Microsoft Teams jest teraz dostępny jako  część nowych instalacji Aplikacje Microsoft 365 dla przedsiębiorstw, Aplikacje Microsoft 365 dla firm i Office dla komputerów Mac. Aby uzyskać więcej informacji, [zobacz Kiedy Microsoft Teams uwzględniane w nowych instalacjach](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps) programu Office?

Ponadto, począwszy od wersji 1906 w bieżącym kanale,  program Teams zostanie dodany do istniejących instalacji programu Aplikacje Microsoft 365 dla przedsiębiorstw (i Aplikacje Microsoft 365 dla firm) na urządzeniach z systemem Windows po zaktualizowaniu istniejącej instalacji do najnowszej wersji. Aby uzyskać więcej informacji, zobacz [Co z istniejącymi instalacjami Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Uwaga:** Jeśli nie chcesz czekać na ten harmonogram wdrożenia, możesz wdrożyć usługę [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) Teams jako autonomiczną dla użytkowników, korzystając z tych instrukcji, lub w celu zainstalowania pakietu Teams dla siebie z [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Jeśli Twoja organizacja nie jest jeszcze gotowa do wdrożenia Teams, mamy kroki, które [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) możesz [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) wykonać, aby wykluczyć Teams z nowych lub istniejących instalacji Office.  Jeśli chcesz Teams, ale nie chcesz, aby program Teams był uruchamiany automatycznie dla użytkownika po jego zainstalowaniu, zobacz Uniemożliwianie automatycznego uruchamiania programu Microsoft Teams po zakończeniu [instalacji.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Aby ***odinstalować Teams*** z urządzenia z systemem Windows, zobacz [Odinstalowywanie Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Aby oczyścić Microsoft Teams z wielu komputerów docelowych lub użytkowników, zobacz Microsoft Teams [oczyszczanie wdrożenia.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Jeśli używasz komputerów udostępnionych, usług pulpitu zdalnego (RDS) lub infrastruktury pulpitów wirtualnych (VDI), zobacz Środowisko komputerów udostępnionych i [środowisk VDI z programem Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Jeśli korzystasz z programu Office dla komputerów Mac, zobacz [Microsoft Teams instalacja na komputerze Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Uwaga:** po Teams jest automatycznie aktualizowana [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) co około dwa tygodnie o nowe funkcje i aktualizacje jakości. 
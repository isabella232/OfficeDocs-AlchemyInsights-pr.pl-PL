---
title: Wdrażanie zespołów jako samodzielny lub z nowych lub istniejących instalacji pakietu Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054240"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Wdrażanie zespołów jako samodzielny lub z nowych lub istniejących instalacji pakietu Office

Teams Microsoft jest teraz dołączone jako część ***nowych instalacji*** pakietu Office 365 ProPlus, Office 365 Business i Office dla komputerów Macintosh. Aby uzyskać więcej informacji, zobacz [Teams Microsoft rozpoczęcia włączane do nowych instalacji pakietu Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Ponadto począwszy od wersji 1906 w kanale co miesiąc, drużyny będą ***dodane do istniejącej instalacji*** pakietu Office 365 ProPlus (i Office 365 Business) na urządzeniach z systemem Windows podczas aktualizacji istniejącej instalacji do najnowszej wersji. Aby uzyskać więcej informacji, zobacz [co z istniejącej instalacji pakietu Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Jeśli nie chcesz czekać na ten harmonogram wdrożenia, można wdrożyć zespołów jako autonomiczny dla użytkowników według [następujących instrukcji](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) lub zlecić swoim użytkownikom instalować zespołów dla siebie z [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Jeśli organizacja nie jest gotowy do wdrożenia zespołów, mamy kroki, które można podjąć, aby ***wykluczyć zespołów*** z [nowej](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) lub [istniejącej](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalacji pakietu Office. Jeśli chcesz zespołom zainstalowana, ale nie ma zespołów do automatycznego uruchamiania dla użytkownika po jego zainstalowaniu, zobacz [Zapobiec zespoły Microsoft uruchamianiu automatycznie po zakończeniu instalacji](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Aby ***odinstalować zespołów*** z urządzenia z systemem Windows zobacz [Odinstalować zespoły pracowników firmy Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Oczyszczanie Teams firmy Microsoft z wielu komputerów docelowych lub użytkowników zobacz [Oczyszczanie wdrażania zespoły pracowników firmy Microsoft](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jeśli używasz udostępnionych komputerów, usług pulpitu zdalnego (RDS) lub infrastruktury pulpitów wirtualnych (VDI), zobacz [współużytkowanego komputera i środowiskach VDI z zespołami firmy Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jeśli używasz pakietu Office dla komputerów Macintosh, zobacz [zespoły Microsoft instalacji na komputerach Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Po zainstalowaniu zespołów jest [automatycznie aktualizowane](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) o nowe funkcje i aktualizacje jakości około dwóch tygodni. 
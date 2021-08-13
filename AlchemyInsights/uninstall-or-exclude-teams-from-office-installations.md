---
title: Odinstalowywanie lub wykluczanie Teams z Office instalacji
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
- "2662"
- "9000660"
ms.openlocfilehash: a960c96abf6215e3a34908ce8669a0c61298daac829343b3673dbfef0c4cbfc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007728"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Odinstalowywanie lub wykluczanie Teams z nowych lub Office instalacji

Microsoft Teams jest uwzględniana jako część Aplikacje Microsoft 365 dla przedsiębiorstw, Aplikacje Microsoft 365 dla firm i Office dla komputerów Mac.

- Użyj narzędzia [Office wdrażania,](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) aby wykluczyć Teams z nowych instalacji pakietu Office.
- Aby *odinstalować* Teams z urządzenia z systemem Windows, zobacz [Odinstalowywanie Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Aby oczyścić Microsoft Teams z wielu komputerów docelowych lub użytkowników, zobacz Microsoft Teams [oczyszczanie wdrożenia.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)
- Użyj opcji [PreventTeamsInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) aby uniemożliwić Microsoft Teams instalacji automatycznie razem z Office.
- Użyj [opcji PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) przed *Teams*, aby uniemożliwić automatyczne uruchamianie Microsoft Teams po zakończeniu instalacji.

Jeśli korzystasz z programu Office dla komputerów Mac, zobacz [Microsoft Teams instalacji na komputerze Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)
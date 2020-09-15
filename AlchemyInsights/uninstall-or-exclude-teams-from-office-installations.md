---
title: Odinstalowywanie lub wykluczanie zespołów z instalacji pakietu Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658231"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Odinstalowywanie lub wykluczanie zespołów z nowych lub istniejących instalacji pakietu Office

Aplikacja Microsoft Teams jest uwzględniona w ramach aplikacji Microsoft 365 Apps dla przedsiębiorstw, aplikacji Microsoft 365 Apps dla firm i pakietu Office dla komputerów Mac.

- Użyj [narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , aby wykluczyć zespoły z nowych instalacji pakietu Office.
- Aby *odinstalować aplikację* Teams z urządzenia z systemem Windows, zobacz [Odinstalowywanie aplikacji Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Aby oczyścić aplikację Microsoft Teams z wielu komputerów docelowych lub użytkowników, zobacz [oczyszczanie wdrażania aplikacji Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Użyj opcji [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) , aby uniemożliwić automatyczne instalowanie aplikacji Microsoft Teams z pakietem Office.
- Przed zainstalowaniem aplikacji *Teams*Użyj opcji [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , aby uniemożliwić automatyczne uruchamianie aplikacji Microsoft Teams po instalacji.

Jeśli korzystasz z pakietu Office dla komputerów Mac, zobacz [instalacje aplikacji Microsoft Teams na komputerze Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).
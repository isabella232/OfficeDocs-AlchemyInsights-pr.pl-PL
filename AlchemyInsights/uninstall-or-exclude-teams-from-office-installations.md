---
title: Odinstalowywanie lub wykluczanie aplikacji Teams z instalacji pakietu Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: b6613733e743e08a9b18b1ada70fde164b0d5dc3
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010309"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Odinstalowywanie lub wykluczanie aplikacji Teams z nowych lub istniejących instalacji pakietu Office

Usługa Microsoft Teams jest częścią usługi Microsoft 365 Apps dla przedsiębiorstw, aplikacji Microsoft 365 dla firm i pakietu Office dla komputerów Mac.

- Narzędzie [wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) umożliwia wykluczenie zespołów z nowych instalacji pakietu Office.
- Aby *odinstalować* usługi Teams z urządzenia z systemem Windows, zobacz [Odinstalowywanie usługi Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Aby oczyścić usługę Microsoft Teams z wielu komputerów docelowych lub użytkowników, zobacz [Oczyszczanie wdrażania usługi Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Użyj opcji [PreventTeamsInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) aby uniemożliwić automatyczne instalowanie usługi Microsoft Teams za pomocą pakietu Office.
- Użyj opcji [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *przed zainstalowaniem programu Teams,* aby zapobiec automatycznemu uruchamianiu usługi Microsoft Teams po instalacji.

Jeśli korzystasz z pakietu Office dla komputerów Mac, zobacz [Instalacje usługi Microsoft Teams na komputerze Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).
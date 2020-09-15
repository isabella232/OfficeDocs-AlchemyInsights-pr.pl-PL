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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="070ba-102">Odinstalowywanie lub wykluczanie zespołów z nowych lub istniejących instalacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="070ba-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="070ba-103">Aplikacja Microsoft Teams jest uwzględniona w ramach aplikacji Microsoft 365 Apps dla przedsiębiorstw, aplikacji Microsoft 365 Apps dla firm i pakietu Office dla komputerów Mac.</span><span class="sxs-lookup"><span data-stu-id="070ba-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="070ba-104">Użyj [narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , aby wykluczyć zespoły z nowych instalacji pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="070ba-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="070ba-105">Aby *odinstalować aplikację* Teams z urządzenia z systemem Windows, zobacz [Odinstalowywanie aplikacji Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="070ba-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="070ba-106">Aby oczyścić aplikację Microsoft Teams z wielu komputerów docelowych lub użytkowników, zobacz [oczyszczanie wdrażania aplikacji Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="070ba-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="070ba-107">Użyj opcji [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) , aby uniemożliwić automatyczne instalowanie aplikacji Microsoft Teams z pakietem Office.</span><span class="sxs-lookup"><span data-stu-id="070ba-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="070ba-108">Przed zainstalowaniem aplikacji *Teams*Użyj opcji [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , aby uniemożliwić automatyczne uruchamianie aplikacji Microsoft Teams po instalacji.</span><span class="sxs-lookup"><span data-stu-id="070ba-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="070ba-109">Jeśli korzystasz z pakietu Office dla komputerów Mac, zobacz [instalacje aplikacji Microsoft Teams na komputerze Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="070ba-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>
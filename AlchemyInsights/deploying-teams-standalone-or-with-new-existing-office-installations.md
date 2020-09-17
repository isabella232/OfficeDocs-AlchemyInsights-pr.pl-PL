---
title: Wdrażanie zespołów jako autonomicznych lub w nowych lub istniejących instalacjach pakietu Office
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806769"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Wdrażanie zespołów jako autonomicznych lub w nowych lub istniejących instalacjach pakietu Office

Aplikacja Microsoft Teams jest teraz dołączona jako część ***nowych instalacji*** aplikacji Microsoft 365 dla przedsiębiorstw, aplikacji Microsoft 365 Apps dla firm i pakietu Office dla komputerów Mac. Aby uzyskać więcej informacji, zobacz [Kiedy pakiet Microsoft Teams zostanie dołączony do nowych instalacji pakietu Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ponadto, począwszy od wersji 1906 w bieżącym kanale, zespoły zostaną ***dodane do istniejących instalacji*** aplikacji Microsoft 365 Apps dla przedsiębiorstw (oraz aplikacji Microsoft 365 dla firm) na urządzeniach z systemem Windows po zaktualizowaniu istniejącej instalacji do najnowszej wersji. Aby uzyskać więcej informacji, zobacz [Omówienie istniejących instalacji pakietu Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Jeśli nie chcesz czekać na ten harmonogram wdrażania, możesz wdrożyć zespoły jako autonomiczne dla użytkowników, postępując zgodnie z [tymi instrukcjami](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   lub możesz mieć możliwość zainstalowania aplikacji Teams przez użytkowników  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Jeśli Twoja organizacja nie jest gotowa do wdrożenia aplikacji Teams, mamy kroki, które można wykonać w celu ***wykluczenia zespołów*** z [nowych](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) lub [istniejących](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalacji pakietu Office. Jeśli chcesz, aby zespoły były instalowane, ale nie chcesz, aby zespoły były uruchamiane automatycznie dla użytkownika po jego zainstalowaniu, zobacz [Zapobieganie automatycznemu uruchamianiu aplikacji Microsoft Teams po instalacji](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Aby ***odinstalować aplikację Teams*** z urządzenia z systemem Windows, zobacz [Odinstalowywanie aplikacji Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Aby oczyścić aplikację Microsoft Teams z wielu komputerów docelowych lub użytkowników, zobacz [oczyszczanie wdrażania aplikacji Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jeśli korzystasz z komputerów udostępnionych, usług pulpitu zdalnego (RDS) lub infrastruktury pulpitów wirtualnych (VDI, Virtual Desktop Infrastructure), zobacz [współużytkowane środowiska komputera i infrastruktury VDI z aplikacją Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jeśli korzystasz z pakietu Office dla komputerów Mac, zobacz [instalacje aplikacji Microsoft Teams na komputerze Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Po zainstalowaniu aplikacji Teams jest ona [automatycznie aktualizowana](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) co dwa tygodnie za pomocą nowych funkcji i aktualizacji jakości. 
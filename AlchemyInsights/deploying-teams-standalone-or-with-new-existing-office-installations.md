---
title: Wdrażanie zespołów jako autonomicznych lub z nowymi lub istniejącymi instalacjami pakietu Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704643"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Wdrażanie zespołów jako autonomicznych lub z nowymi lub istniejącymi instalacjami pakietu Office

Usługa Microsoft Teams jest teraz dostępna jako część ***nowych instalacji*** aplikacji microsoft 365 dla przedsiębiorstw, aplikacji Microsoft 365 dla firm i pakietu Office dla komputerów Mac. Aby uzyskać więcej informacji, zobacz [Kiedy usługa Microsoft Teams zacznie być dołączona do nowych instalacji pakietu Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Ponadto począwszy od wersji 1906 w kanale miesięcznym usługa Teams zostanie ***dodana do istniejących instalacji*** aplikacji microsoft 365 dla przedsiębiorstw (i aplikacji microsoft 365 dla firm) na urządzeniach z systemem Windows podczas aktualizowania istniejącej instalacji do najnowszej wersji. Aby uzyskać więcej informacji, zobacz [Co z istniejącymi instalacjami pakietu Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Jeśli nie chcesz czekać na ten harmonogram wdrażania, możesz wdrożyć usługi Teams jako samodzielne dla użytkowników, [postępując zgodnie](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)z tymi instrukcjami lub możesz poprosić użytkowników o zainstalowanie zespołów dla siebie z programu .

Jeśli Twoja organizacja nie jest gotowa do wdrożenia usługi Teams, mamy kroki, które można wykonać, aby ***wykluczyć usługi Teams*** z [nowych](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) lub [istniejących](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalacji pakietu Office. Jeśli chcesz, aby usługa Teams była instalowana, ale nie chcesz, aby usługa Teams uruchamiała się automatycznie dla użytkownika po jego zainstalowaniu, zobacz [Zapobieganie automatycznemu uruchamianiu usługi Microsoft Teams po instalacji](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Aby ***odinstalować usługi Teams*** z urządzenia z systemem Windows, zobacz [Odinstalowywanie usługi Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Aby oczyścić usługę Microsoft Teams z wielu komputerów docelowych lub użytkowników, zobacz [Oczyszczanie wdrażania usługi Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jeśli używasz komputerów udostępnionych, usług pulpitu zdalnego (RDS) lub infrastruktury pulpitu wirtualnego (VDI), zobacz [Udostępnione środowiska komputerów i środowisk VDI w usłudze Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jeśli korzystasz z pakietu Office dla komputerów Mac, zobacz [Instalacje usługi Microsoft Teams na komputerze Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Po zainstalowaniu aplikacji Teams jest ona [automatycznie aktualizowana](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) co około dwa tygodnie za pomocą nowych funkcji i aktualizacji jakości. 
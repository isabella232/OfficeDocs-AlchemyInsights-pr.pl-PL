---
title: Instalowanie pakietu Office na serwerze terminali — bez licencji
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010624"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalowanie pakietu Office na serwerze terminali

Aby wdrożyć aplikacje usługi Microsoft 365 dla przedsiębiorstw w systemie Windows Server przy użyciu usług pulpitu zdalnego (RDS), wcześniej nazwanych usługami terminalowymi:
  
- Musisz mieć subskrypcję usługi Microsoft 365, która obejmuje aplikacje microsoft 365 dla przedsiębiorstw, takie jak Office 365 Enterprise E3 lub Enterprise E5. Plany microsoft 365 Apps dla firm i Microsoft 365 Apps for business Premium nie obejmują aplikacji Microsoft 365 dla przedsiębiorstw.

- Należy włączyć [aktywację komputera współdzielonego](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Jeśli chcesz zainstalować usługę Microsoft 365 Apps dla przedsiębiorstw na usługach RDS z centrum administracyjnego usługi Microsoft 365, ***które używa domyślnych ustawień instalacji,*** należy wykonać następujące czynności.

> [!TIP]
> Można również pobrać i uruchomić [Asystenta pomocy technicznej i odzyskiwania firmy Microsoft,](https://aka.ms/SaRA_OfficeSCA_M365Portal) aby zainstalować aplikacje microsoft 365 dla przedsiębiorstwa w trybie aktywacji komputera udostępnionego.
  
1. Sprawdź, jaką masz subskrypcję usługi Microsoft 365. [Dowiedz się, jak](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. W razie potrzeby przełącz się na inną subskrypcję usługi Microsoft 365. [Dowiedz się, jak](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Jeśli pakiet Office jest już zainstalowany na serwerze usług pulpitu zdalnego przy użyciu innych subskrypcji usługi Microsoft 365, odinstaluj go. Na przykład, przechodząc do \> Panelu sterowania Odinstaluj program. Odinstaluj za pomocą [Pomocy technicznej firmy Microsoft i Asystenta odzyskiwania,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jeśli występują problemy.

4. Na serwerze usług pulpitu zdalnego zaloguj się do centrum administracyjnego usługi Microsoft 365 za pomocą konta administratora i [zainstaluj aplikację Microsoft 365 Apps dla przedsiębiorstw](https://portal.office.com/OLS/MySoftware.aspx).

5. Po zainstalowaniu pakietu Office ***nie otwieraj ani nie loguj*** się do żadnych aplikacji pakietu Office.

6. Na serwerze usług pulpitu zdalnego włącz aktywację komputera udostępnionego, edytując rejestr, wykonując następujące czynności:

1. Kliknij prawym przyciskiem myszy przycisk Windows w lewym dolnym rogu ekranu i wybierz pozycję Uruchom. W polu Otwórz wpisz **regedit**, a następnie wybierz przycisk OK.

2. Wybierz pozycję Tak po wyświetleniu monitu, aby zezwolić Edytorowi rejestru na wprowadzanie zmian na urządzeniu.

3. W Edytorze rejestru dodaj wartość ciągu **SharedComputerLicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na serwerze usług pulpitu ***zdalnego zaloguj się jako użytkownik końcowy*** i [sprawdź, czy aktywacja udostępnionego komputera jest włączona dla aplikacji usługi Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Aby uzyskać więcej informacji na temat wymagań wstępnych, instrukcji konfiguracji i wskazówek dotyczących niestandardowych instalacji przy użyciu Narzędzia wdrażania pakietu Office, zobacz [Wdrażanie aplikacji microsoft 365 dla przedsiębiorstw przy użyciu usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Aby naprawić błędy związane z aktywacją komputera współdzielonego, zobacz [Rozwiązywanie problemów z aktywacją komputera udostępnionego dla aplikacji usługi Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  
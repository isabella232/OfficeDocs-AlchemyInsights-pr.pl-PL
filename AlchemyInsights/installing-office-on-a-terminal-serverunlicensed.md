---
title: Instalowanie pakietu Office na serwerze terminali — nielicencjonowane
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322009"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalowanie Office na serwerze terminali

Do wdrażania Aplikacje Microsoft 365 dla przedsiębiorstw na serwerze Windows przy użyciu usług pulpitu zdalnego (RDS), dawniej nazwanych usługami terminalowych:
  
- Musisz mieć subskrypcję usługi Microsoft 365, która obejmuje Aplikacje Microsoft 365 dla przedsiębiorstw, na przykład Office 365 Enterprise E3 lub Enterprise E5. Plany Aplikacje Microsoft 365 dla firm i Aplikacje Microsoft 365 dla firm Premium nie obejmują Aplikacje Microsoft 365 dla przedsiębiorstw.

- Musisz włączyć aktywację [na komputerze udostępnionym.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Jeśli chcesz zainstalować oprogramowanie w Aplikacje Microsoft 365 dla przedsiębiorstw RDS z serwera ***centrum administracyjne platformy Microsoft 365,*** w którym są używane ustawienia domyślne instalacji, należy wykonać następujące czynności.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Sprawdź, Microsoft 365 posiadasz subskrypcję. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. W razie potrzeby zmień subskrypcję na Microsoft 365 subskrypcji. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jeśli Office jest już zainstalowany na serwerze RDS przy użyciu innych Microsoft 365, odinstaluj go. Na przykład, przechodząc do panelu sterowania \> Odinstalowywanie programu. Jeśli masz [problemy Asystent odzyskiwania i pomocy technicznej](https://aka.ms/SARA-OfficeUninstall-Alchemy) odinstaluj aplikację Microsoft Asystent odzyskiwania i pomocy technicznej.

4. Na serwerze RDS zaloguj się do strony centrum administracyjne platformy Microsoft 365 za pomocą konta administratora i [zainstaluj](https://portal.office.com/OLS/MySoftware.aspx)Aplikacje Microsoft 365 dla przedsiębiorstw.

5. Po Office nie otwieraj żadnych aplikacji ani nie ***loguj*** się do Office aplikacji.

6. Na serwerze RDS włącz aktywację komputera udostępnionego, edytując rejestr, korzystając z następujących kroków:

1. Kliknij prawym przyciskiem myszy przycisk Windows w lewym dolnym rogu ekranu i wybierz polecenie Uruchom. W polu Otwórz wpisz **polecenie regedit**, a następnie wybierz przycisk OK.

2. Po wyświetleniu monitu o umożliwienie Edytorowi rejestru zmiany na urządzeniu wybierz pozycję Tak.

3. W Edytorze rejestru dodaj wartość ciągu **SharedComputerLicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na serwerze RDS zaloguj się jako użytkownik ***końcowy*** i sprawdź, czy aktywacja na komputerze udostępnionym [jest](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)włączona dla Aplikacje Microsoft 365 dla przedsiębiorstw.

Aby uzyskać więcej szczegółowych informacji na temat wymagań wstępnych, instrukcji konfiguracji i wskazówek dotyczących instalacji dostosowanych przy użyciu Narzędzia wdrażania Office, zobacz Wdrażanie usługi Aplikacje Microsoft 365 dla przedsiębiorstw przy użyciu usług pulpitu [zdalnego.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Aby naprawić błędy związane z aktywacją komputera udostępnionego, zobacz Rozwiązywanie problemów z aktywacją na komputerze udostępnionym dla użytkowników [Aplikacje Microsoft 365 dla przedsiębiorstw.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  
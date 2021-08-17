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
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055168"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalowanie Office na serwerze terminali

Do wdrażania Aplikacje Microsoft 365 dla przedsiębiorstw na serwerze Windows przy użyciu usług pulpitu zdalnego (RDS), dawniej nazwanych usługami terminalowych:
  
- Musisz mieć subskrypcję usługi Microsoft 365, która obejmuje Aplikacje Microsoft 365 dla przedsiębiorstw, taką jak Office 365 Enterprise E3 lub Enterprise E5. Plany Aplikacje Microsoft 365 dla firm i Aplikacje Microsoft 365 dla firm Premium nie obejmują Aplikacje Microsoft 365 dla przedsiębiorstw.

- Musisz włączyć aktywację [na komputerze udostępnionym.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Jeśli chcesz zainstalować oprogramowanie Aplikacje Microsoft 365 dla przedsiębiorstw RDS z ***centrum administracyjne platformy Microsoft 365,*** w którym są używane domyślne ustawienia instalacji, należy wykonać następujące czynności.

> [!TIP]
> Możesz również pobrać i uruchomić aplikację [Microsoft Asystent odzyskiwania i pomocy technicznej,](https://aka.ms/SaRA_OfficeSCA_M365Portal) aby Aplikacje Microsoft 365 dla przedsiębiorstw w trybie aktywacji komputera udostępnionego.
  
1. Sprawdź, Microsoft 365 posiadasz subskrypcję. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. W razie potrzeby zmień subskrypcję na inną Microsoft 365 subskrypcji. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jeśli Office na serwerze RDS przy użyciu innych Microsoft 365, odinstaluj go. Na przykład, przechodząc do panelu sterowania \> Odinstalowywanie programu. Jeśli masz [problemy Asystent odzyskiwania i pomocy technicznej](https://aka.ms/SARA-OfficeUninstall-Alchemy) odinstalowywanie przy użyciu programu Microsoft Asystent odzyskiwania i pomocy technicznej.

4. Na serwerze RDS zaloguj się do witryny sieci centrum administracyjne platformy Microsoft 365 za pomocą konta administratora i zainstaluj [Aplikacje Microsoft 365 dla przedsiębiorstw.](https://portal.office.com/OLS/MySoftware.aspx)

5. Po Office nie ***otwieraj żadnych*** aplikacji ani nie loguj się do Office aplikacji.

6. Na serwerze RDS włącz aktywację komputera udostępnionego, edytując rejestr, korzystając z następujących kroków:

1. Kliknij prawym przyciskiem myszy przycisk Windows w lewym dolnym rogu ekranu i wybierz polecenie Uruchom. W polu Otwórz wpisz **polecenie regedit**, a następnie wybierz przycisk OK.

2. Po wyświetleniu monitu o umożliwienie Edytorowi rejestru zmiany na urządzeniu wybierz pozycję Tak.

3. W Edytorze rejestru dodaj wartość ciągu **SharedComputerLicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na serwerze RDS zaloguj się jako użytkownik ***końcowy*** i upewnij się, że włączono aktywację komputera [Aplikacje Microsoft 365 dla przedsiębiorstw.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Aby uzyskać więcej szczegółowych informacji na temat wymagań wstępnych, instrukcji konfiguracji i wskazówek dotyczących instalacji dostosowanych przy użyciu Narzędzia wdrażania Office, zobacz Wdrażanie usługi Aplikacje Microsoft 365 dla przedsiębiorstw przy użyciu usług pulpitu [zdalnego.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Aby naprawić błędy związane z aktywacją na komputerze udostępnionym, zobacz Rozwiązywanie problemów z aktywacją na komputerze udostępnionym dla [użytkowników Aplikacje Microsoft 365 dla przedsiębiorstw.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  
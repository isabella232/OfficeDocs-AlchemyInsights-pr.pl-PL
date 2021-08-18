---
title: Wdrażanie Aplikacje Microsoft 365 dla przedsiębiorstw do użytku udostępnionego w rds, serwerze terminali lub VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325613"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Wdrażanie Aplikacje Microsoft 365 dla przedsiębiorstw do użytku udostępnionego w rds, serwerze terminali lub VDI

Aby wdrożyć Aplikacje Microsoft 365 dla przedsiębiorstw usług pulpitu zdalnego (RDS), wcześniej nazwanych usług terminalowych:

- Musisz mieć plan usługi Microsoft 365 dla firm lub plan Office 365 usługi Aplikacje Microsoft 365 dla przedsiębiorstw, taki jak Office 365 Enterprise E3 lub Enterprise E5.
   **Uwaga:** plany Aplikacje Microsoft 365 dla firm i Microsoft 365 Business Standard nie obejmują Aplikacje Microsoft 365 dla przedsiębiorstw.
- Należy włączyć [aktywację na komputerze udostępnionym.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**Uwaga:** Możesz również pobrać i uruchomić aplikację [Microsoft Asystent odzyskiwania i pomocy technicznej,](https://aka.ms/SaRA_OfficeSCA_M365Portal) aby zainstalować Aplikacje Microsoft 365 dla przedsiębiorstw w trybie aktywacji na komputerze udostępnionym.

Aby uzyskać więcej informacji na temat wymagań wstępnych, instrukcji konfiguracji i wskazówek dotyczących instalacji dostosowanych przy użyciu Narzędzia wdrażania Office, zobacz Wdrażanie usługi Aplikacje Microsoft 365 dla przedsiębiorstw przy użyciu usług pulpitu [zdalnego.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Aby naprawić błędy związane z aktywacją na komputerze udostępnionym:

- Zobacz [Rozwiązywanie problemów z aktywacją komputera udostępnionego na Aplikacje Microsoft 365 dla przedsiębiorstw.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Zobacz [Resetowanie stanu aktywacji aplikacji subskrypcji Aplikacje Microsoft 365 dla przedsiębiorstw](https://go.microsoft.com/fwlink/?linkid=2109218).

Jeśli chcesz zainstalować oprogramowanie Aplikacje Microsoft 365 dla przedsiębiorstw RDS z ***centrum administracyjne platformy Microsoft 365,*** w którym są używane ustawienia domyślne instalacji, należy wykonać następujące czynności:

1. Sprawdź posiadaną subskrypcję. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. W razie potrzeby zmień subskrypcję na inną. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Jeśli Office na serwerze RDS przy użyciu innych subskrypcji firmy Microsoft, odinstaluj go. Na przykład, przechodząc do **panelu sterowania**  >  **Odinstaluj program**. Jeśli masz [problemy Asystent odzyskiwania i pomocy technicznej](https://aka.ms/SARA-OfficeUninstall-Alchemy) odinstaluj aplikację Microsoft Asystent odzyskiwania i pomocy technicznej.
4. Na serwerze RDS zaloguj się do strony centrum administracyjne platformy Microsoft 365 za pomocą konta administratora i [zainstaluj](https://portal.office.com/OLS/MySoftware.aspx)Aplikacje Microsoft 365 dla przedsiębiorstw.
5. Po Office nie otwieraj żadnych aplikacji ani nie ***loguj*** się do Office aplikacji.
6. Na serwerze RDS włącz aktywację komputera udostępnionego, edytując rejestr, korzystając z następujących kroków:
   1. Kliknij prawym przyciskiem myszy Windows w lewym dolnym rogu ekranu, a następnie wybierz polecenie **Uruchom**. W polu Otwórz wpisz polecenie **regedit**, a następnie kliknij przycisk **OK**.
   2. Po **wyświetleniu** monitu o umożliwienie Edytorowi rejestru zmiany na urządzeniu wybierz pozycję Tak.
   3. W Edytorze rejestru dodaj wartość ciągu **SharedComputerLicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serwerze RDS zaloguj się jako użytkownik ***końcowy*** i sprawdź, czy aktywacja na komputerze udostępnionym [jest](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)włączona dla Aplikacje Microsoft 365 dla przedsiębiorstw.

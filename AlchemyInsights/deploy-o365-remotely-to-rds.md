---
title: Wdrażanie aplikacji platformy Microsoft 365 dla przedsiębiorstw do użytku udostępnionego w usługach RDS, Terminal Server lub VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200683"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Wdrażanie aplikacji platformy Microsoft 365 dla przedsiębiorstw do użytku udostępnionego w usługach RDS, Terminal Server lub VDI

Aby wdrożyć aplikacje platformy Microsoft 365 dla przedsiębiorstw przy użyciu usług pulpitu zdalnego (RDS), wcześniej nazwanych usługami terminalowych:

- Musisz mieć plan platformy Microsoft 365 dla firm lub plan usługi Office 365, który zawiera aplikacje platformy Microsoft 365 dla przedsiębiorstw, na przykład Office 365 Enterprise E3 lub Enterprise E5.
   > [!NOTE]
   > Plany aplikacje Microsoft 365 dla firm i Microsoft 365 Business Standard nie obejmują aplikacji platformy Microsoft 365 dla przedsiębiorstw.
- Należy włączyć [aktywację na komputerze udostępnionym.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Możesz również pobrać i uruchomić Asystenta odzyskiwania i pomocy technicznej firmy [Microsoft,](https://aka.ms/SaRA_OfficeSCA_M365Portal) aby zainstalować aplikacje Microsoft 365 dla przedsiębiorstw w trybie aktywacji komputera udostępnionego.

Aby uzyskać więcej informacji na temat wymagań wstępnych, instrukcji konfiguracji i wskazówek dotyczących instalacji dostosowanych przy użyciu Narzędzia wdrażania pakietu Office, zobacz Wdrażanie aplikacji [platformy Microsoft 365](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)dla przedsiębiorstw przy użyciu usług pulpitu zdalnego.

Aby naprawić błędy związane z aktywacją na komputerze udostępnionym:

- Zobacz [Rozwiązywanie problemów z aktywacją na komputerze udostępnionym w aplikacjach platformy Microsoft 365 dla przedsiębiorstw.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Zobacz [Resetowanie stanu aktywacji aplikacji subskrypcji Aplikacje Microsoft 365 dla przedsiębiorstw](https://go.microsoft.com/fwlink/?linkid=2109218).

Jeśli chcesz zainstalować aplikacje Platformy Microsoft 365 dla przedsiębiorstw na rds z centrum administracyjnego platformy Microsoft 365, które korzysta z domyślnych ustawień instalacji, należy wykonać następujące czynności:

1. Sprawdź posiadaną subskrypcję. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. W razie potrzeby zmień subskrypcję na inną. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Jeśli pakiet Office jest już zainstalowany na serwerze RDS przy użyciu innych subskrypcji firmy Microsoft, odinstaluj go. Na przykład, przechodząc do **panelu sterowania**  >  **Odinstaluj program**. Jeśli masz problemy, odinstaluj konto przy użyciu Asystenta odzyskiwania i pomocy technicznej firmy [Microsoft.](https://aka.ms/SARA-OfficeUninstall-Alchemy)
4. Na serwerze RDS zaloguj się do centrum administracyjnego platformy Microsoft 365 przy użyciu konta administratora i zainstaluj aplikacje [platformy Microsoft 365 dla przedsiębiorstw.](https://portal.office.com/OLS/MySoftware.aspx)
5. Po zainstalowaniu pakietu Office nie otwieraj żadnych aplikacji pakietu Office ani nie ***loguj*** się do tych aplikacji.
6. Na serwerze RDS włącz aktywację komputera udostępnionego, edytując rejestr, korzystając z następujących kroków:
   1. Kliknij prawym przyciskiem myszy przycisk systemu Windows w lewym dolnym rogu ekranu i wybierz polecenie **Uruchom**. W polu Otwórz wpisz polecenie **regedit**, a następnie kliknij przycisk **OK**.
   2. Po **wyświetleniu** monitu o umożliwienie Edytorowi rejestru zmiany na urządzeniu wybierz pozycję Tak.
   3. W Edytorze rejestru dodaj wartość ciągu **SharedComputerLicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serwerze RDS ***zaloguj*** się jako użytkownik końcowy i sprawdź, czy włączono aktywację na komputerze udostępnionym dla aplikacji [platformy Microsoft 365 dla przedsiębiorstw.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

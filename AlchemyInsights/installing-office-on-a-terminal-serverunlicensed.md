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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205419"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalowanie pakietu Office na serwerze terminali

Aby wdrożyć pakiet Office 365 ProPlus w systemie Windows Server przy użyciu usług pulpitu zdalnego (RDS), dawniej nazywanych usługami terminalowymi:
  
- Musi mieć plan 365 pakietu Office, który zawiera pakiet Office 365 ProPlus, takich jak Office 365 Enterprise E3 lub Enterprise E5. Plany Office 365 Business i Office 365 Business Premium nie zawierają pakietu Office 365 ProPlus.

- Należy włączyć [aktywację udostępnionego komputera](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Jeśli chcesz zainstalować pakiet Office 365 ProPlus na RDS z centrum administracyjnego Microsoft 365, ***które używa domyślnych ustawień instalacji***, wykonaj następujące kroki.

> [!TIP]
> Można również pobrać i uruchomić [Microsoft Support i Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) do zainstalowania pakietu Office 365 ProPlus w trybie aktywacji komputera udostępnionego.
  
1. Sprawdź, co masz plan 365 Office. [Dowiedz się, jak](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Jeśli to konieczne, przełącz się do innego pakietu Office 365 plan. [Dowiedz się, jak](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Jeśli pakiet Office jest już zainstalowany na serwerze usług pulpitu zdalnego przy użyciu innych planów pakietu Office 365, odinstaluj go. Na przykład, przechodząc do panelu \> sterowania Odinstaluj program. Odinstaluj, korzystając z [pomocy technicznej firmy Microsoft i asystenta odzyskiwania](https://aka.ms/SARA-OfficeUninstall-Alchemy) , jeśli masz problemy z uruchamianiem.

4. Na serwerze RDS Zaloguj się do centrum administracyjnego Microsoft 365 z kontem administratora i [Zainstaluj pakiet Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Po zainstalowaniu pakietu Office ***nie otwieraj ani nie logujesz*** się do żadnych aplikacji pakietu Office.

6. Na serwerze usług pulpitu zdalnego Włącz aktywację udostępnionego komputera, edytując rejestr, wykonując następujące kroki:

1. Kliknij prawym przyciskiem myszy przycisk Windows w lewym dolnym rogu ekranu i wybierz polecenie Uruchom. W polu Otwórz wpisz **regedit**, a następnie wybierz przycisk OK.

2. Wybierz opcję tak po wyświetleniu monitu, aby zezwolić edytorowi rejestru na wprowadzanie zmian w urządzeniu.

3. W Edytorze rejestru Dodaj wartość ciągu **Sharedcomputerlicensing** z ustawieniem 1 pod HKEY_LOCAL_MACHINE\Software\Microsoft \Office\ClickToRun\Configuration.

7. Na serwerze usług pulpitu zdalnego ***Zaloguj się jako użytkownik końcowy*** i [Sprawdź, czy aktywacja udostępnionego komputera jest włączona dla pakietu Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Aby uzyskać więcej informacji na temat wymagań wstępnych, instrukcje instalacji i wskazówki dotyczące instalacji dostosowanych za pomocą narzędzia wdrażania pakietu Office, zobacz [wdrażanie pakietu office 365 ProPlus przy użyciu usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Aby naprawić błędy związane z aktywacją komputera udostępnionego, zobacz [Rozwiązywanie problemów z aktywacją komputera udostępnionego dla pakietu Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  
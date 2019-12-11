---
title: Wdrażanie pakietu Office 365 ProPlus do użytku udostępnionego na RDS, Terminal Server lub VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959469"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Wdrażanie pakietu Office 365 ProPlus do użytku udostępnionego na RDS, Terminal Server lub VDI

Aby wdrożyć pakiet Office 365 ProPlus przy użyciu usług pulpitu zdalnego (RDS), dawniej nazwanych usług terminalowych:
- Musi mieć Microsoft 365 dla biznesplanu lub Office 365 plan, który zawiera Office 365 ProPlus, takich jak Office 365 Enterprise E3 lub Enterprise E5.
   > [!NOTE] 
   > Plany Office 365 Business i Office 365 Business Premium nie zawierają pakietu Office 365 ProPlus.
- Należy włączyć [aktywację udostępnionego komputera](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Można również pobrać i uruchomić [Microsoft Support i Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) do zainstalowania pakietu Office 365 ProPlus w trybie aktywacji komputera udostępnionego.

Aby uzyskać więcej informacji na temat wymagań wstępnych, instrukcje dotyczące instalacji i wskazówki dotyczące instalacji dostosowanych za pomocą narzędzia wdrażania pakietu Office, zobacz [wdrażanie pakietu office 365 ProPlus przy użyciu usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Aby naprawić błędy związane z aktywacją komputera udostępnionego:
- Zobacz [Rozwiązywanie problemów z aktywacją komputera udostępnionego dla pakietu Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Zobacz [resetowanie stanu aktywacji pakietu Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Jeśli chcesz zainstalować pakiet Office 365 ProPlus na RDS z centrum administracyjnego Microsoft 365, ***które używa domyślnych ustawień instalacji***, wykonaj następujące czynności:

1.  Sprawdź, co masz plan 365 Office. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Jeśli to konieczne, przełącz się do innego pakietu Office 365 plan. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Jeśli pakiet Office jest już zainstalowany na serwerze usług pulpitu zdalnego przy użyciu innych planów pakietu Office 365, odinstaluj go. Na przykład, przechodząc do **panelu** > sterowania**Odinstaluj program**. Odinstaluj, korzystając z [pomocy technicznej firmy Microsoft i asystenta odzyskiwania](https://aka.ms/SARA-OfficeUninstall-Alchemy) , jeśli masz problemy z uruchamianiem.
4.  Na serwerze RDS Zaloguj się do centrum administracyjnego Microsoft 365 z kontem administratora i [Zainstaluj pakiet Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Po zainstalowaniu pakietu Office ***nie otwieraj ani nie logujesz*** się do żadnych aplikacji pakietu Office.
6.  Na serwerze usług pulpitu zdalnego Włącz aktywację udostępnionego komputera, edytując rejestr, wykonując następujące kroki:
   1. Kliknij prawym przyciskiem myszy przycisk Windows znajdujący się w lewym dolnym rogu ekranu i wybierz polecenie **Uruchom**. W polu Otwórz wpisz **polecenie regedit**, a następnie wybierz **przycisk OK**.
   2. Wybierz opcję **tak** po wyświetleniu monitu, aby zezwolić edytorowi rejestru na wprowadzanie zmian w urządzeniu.
   3. W Edytorze rejestru Dodaj wartość ciągu **Sharedcomputerlicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serwerze usług pulpitu zdalnego ***Zaloguj się jako użytkownik końcowy*** i [Sprawdź, czy aktywacja udostępnionego komputera jest włączona dla pakietu Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).


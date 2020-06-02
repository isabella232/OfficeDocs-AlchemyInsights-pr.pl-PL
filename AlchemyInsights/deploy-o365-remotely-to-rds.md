---
title: Wdrażanie aplikacji usługi Microsoft 365 dla przedsiębiorstw do użytku współużytkującego na serwerze rds, serwerze terminali lub vdi
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507596"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Wdrażanie aplikacji usługi Microsoft 365 dla przedsiębiorstw do użytku współużytkującego na serwerze rds, serwerze terminali lub vdi

Aby wdrożyć aplikacje usługi Microsoft 365 dla przedsiębiorstw przy użyciu usług pulpitu zdalnego (RDS), dawniej nazwanych usługami terminalowymi:
- Musisz mieć plan usługi Microsoft 365 dla firm lub plan usługi Office 365 obejmujący aplikacje usługi Microsoft 365 dla przedsiębiorstw, takie jak Office 365 Enterprise E3 lub Enterprise E5.
   > [!NOTE] 
   > Plany microsoft 365 Apps dla firm i Microsoft 365 Business Premium Standard nie obejmują aplikacji Microsoft 365 dla przedsiębiorstw.
- Należy włączyć [aktywację komputera udostępnionego](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Można również pobrać i uruchomić [Asystenta pomocy technicznej i odzyskiwania firmy Microsoft,](https://aka.ms/SaRA_OfficeSCA_M365Portal) aby zainstalować aplikacje microsoft 365 dla przedsiębiorstwa w trybie aktywacji komputera udostępnionego.

Aby uzyskać więcej informacji na temat wymagań wstępnych, instrukcji konfiguracji i wskazówek dotyczących niestandardowych instalacji przy użyciu Narzędzia wdrażania pakietu Office, zobacz [Wdrażanie aplikacji usługi Microsoft 365 dla przedsiębiorstw przy użyciu usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Aby naprawić błędy związane z aktywacją udostępnionego komputera:
- Zobacz [Rozwiązywanie problemów z aktywacją komputera udostępnionego dla aplikacji usługi Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Zobacz [Resetowanie stanu aktywacji aplikacji subskrypcji Aplikacje Microsoft 365 dla przedsiębiorstw](https://go.microsoft.com/fwlink/?linkid=2109218).

Jeśli chcesz zainstalować usługę Microsoft 365 Apps dla przedsiębiorstw na usługach rds z centrum administracyjnego usługi Microsoft 365, ***które używa domyślnych ustawień instalacji,*** należy wykonać następujące czynności:

1.    Sprawdź, jaką masz subskrypcję. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    W razie potrzeby przełącz się na inną subskrypcję. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Jeśli pakiet Office jest już zainstalowany na serwerze usług pulpitu zdalnego przy użyciu innych subskrypcji firmy Microsoft, odinstaluj go. Na przykład, przechodząc do **Panelu sterowania**  >  **Odinstaluj program**. Odinstaluj za pomocą [Pomocy technicznej firmy Microsoft i Asystenta odzyskiwania,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jeśli występują problemy.
4.    Na serwerze usług pulpitu zdalnego zaloguj się do centrum administracyjnego usługi Microsoft 365 za pomocą konta administratora i [zainstaluj aplikację Microsoft 365 Apps dla przedsiębiorstw](https://portal.office.com/OLS/MySoftware.aspx).
5.    Po zainstalowaniu pakietu Office ***nie otwieraj ani nie loguj*** się do żadnych aplikacji pakietu Office.
6.    Na serwerze usług pulpitu zdalnego włącz aktywację komputera udostępnionego, edytując rejestr, wykonując następujące czynności:
   1. Kliknij prawym przyciskiem myszy przycisk Windows w lewym dolnym rogu ekranu i wybierz polecenie **Uruchom**. W polu Otwórz wpisz **regedit**, a następnie wybierz przycisk **OK**.
   2. Wybierz **pozycję Tak** po wyświetleniu monitu, aby zezwolić Edytorowi rejestru na wprowadzanie zmian na urządzeniu.
   3. W Edytorze rejestru dodaj wartość ciągu **SharedComputerLicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serwerze usług pulpitu ***zdalnego zaloguj się jako użytkownik końcowy*** i [sprawdź, czy aktywacja udostępnionego komputera jest włączona dla aplikacji usługi Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).


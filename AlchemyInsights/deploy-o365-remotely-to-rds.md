---
title: Wdrażanie aplikacji Microsoft 365 dla przedsiębiorstw do współużytkowania na serwerach RDS, serwer terminali lub VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745545"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Wdrażanie aplikacji Microsoft 365 dla przedsiębiorstw do współużytkowania na serwerach RDS, serwer terminali lub VDI

Aby wdrożyć aplikacje Microsoft 365 dla przedsiębiorstw przy użyciu usług pulpitu zdalnego (RDS), dawniej nazwane usługi terminalowe:
- Musisz mieć plan Microsoft 365 dla firm lub plan pakietu Office 365, który zawiera aplikacje Microsoft 365 dla przedsiębiorstw, takie jak Office 365 Enterprise E3 lub Enterprise E5.
   > [!NOTE] 
   > Pakiet Microsoft 365 Apps dla firm i Microsoft 365 Business Premium Standard nie zawierają aplikacji Microsoft 365 Apps dla przedsiębiorstw.
- Musisz włączyć [aktywację komputera współużytkowanego](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Możesz również pobrać i uruchomić [asystenta odzyskiwania i pomocy technicznej firmy Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) w celu zainstalowania aplikacji Microsoft 365 Apps dla przedsiębiorstw w trybie aktywacji komputerów współużytkowanych.

Aby uzyskać więcej informacji na temat wymagań wstępnych, instrukcji dotyczących konfiguracji i wskazówek dotyczących instalacji niestandardowych przy użyciu narzędzia wdrażania pakietu Office, zobacz [wdrażanie aplikacji Microsoft 365 dla przedsiębiorstw za pomocą usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Aby naprawić błędy związane z aktywacją na komputerze współużytkowanym:
- Zobacz [Rozwiązywanie problemów z aktywacją udostępniania komputera dla aplikacji Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Zobacz [Resetowanie stanu aktywacji aplikacji subskrypcji Aplikacje Microsoft 365 dla przedsiębiorstw](https://go.microsoft.com/fwlink/?linkid=2109218).

Jeśli chcesz zainstalować aplikacje Microsoft 365 dla przedsiębiorstw na komputerze RDS z centrum administracyjnego Microsoft 365, ***które korzysta z domyślnych ustawień instalacji***, wykonaj następujące czynności:

1.    Sprawdź, jakie posiadasz abonament. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Jeśli to konieczne, przejdź do innej subskrypcji. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Jeśli pakiet Office jest już zainstalowany na serwerze RDS przy użyciu innych abonamentów firmy Microsoft, odinstaluj go. Na przykład, przechodząc do **Panelu sterowania**,  >  **Odinstaluj program**. Odinstaluj za pomocą [asystenta odzyskiwania i pomocy technicznej firmy Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) , jeśli występują problemy.
4.    Na serwerze RDS Zaloguj się do centrum administracyjnego usługi Microsoft 365 przy użyciu konta administratora i [Zainstaluj aplikację Microsoft 365 Apps dla przedsiębiorstw](https://portal.office.com/OLS/MySoftware.aspx).
5.    Po zainstalowaniu pakietu Office ***nie otwieraj ani nie loguj*** się do żadnych aplikacji pakietu Office.
6.    Na serwerze RDS Włącz aktywację komputera udostępnionego, edytując rejestr, wykonując następujące czynności:
   1. Kliknij prawym przyciskiem myszy przycisk systemu Windows w lewym dolnym rogu ekranu i wybierz polecenie **Uruchom**. W polu Otwórz wpisz ciąg **regedit**, a następnie wybierz przycisk **OK**.
   2. Wybierz pozycję **tak** , gdy zostanie wyświetlony monit o zezwolenie na wprowadzanie zmian na urządzeniu przez Edytor rejestru.
   3. W Edytorze rejestru Dodaj wartość ciągu **SharedComputerLicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Na serwerze RDS ***Zaloguj się jako użytkownik końcowy*** i [upewnij się, że Aktywacja komputera udostępnionego jest włączona dla aplikacji Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).


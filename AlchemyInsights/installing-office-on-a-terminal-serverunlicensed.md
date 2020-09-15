---
title: Instalowanie pakietu Office na serwerze terminali — bez licencji
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663127"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalowanie pakietu Office na serwerze terminali

Wdrażanie aplikacji Microsoft 365 dla przedsiębiorstw na serwerze z systemem Windows przy użyciu usług pulpitu zdalnego (RDS) — dawniej nazywane usługami terminalowymi:
  
- Musisz mieć subskrypcję programu Microsoft 365 obejmującą aplikacje Microsoft 365 dla przedsiębiorstw, takie jak Office 365 Enterprise E3 lub Enterprise E5. Pakiet Microsoft 365 Apps dla firm i aplikacje Microsoft 365 dla firm w wersji Premium nie zawierają aplikacji Microsoft 365 Apps dla przedsiębiorstw.

- Musisz włączyć [aktywację komputera współużytkowanego](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Jeśli chcesz zainstalować aplikacje Microsoft 365 dla przedsiębiorstw na komputerze RDS z centrum administracyjnego Microsoft 365, ***które korzysta z domyślnych ustawień instalacji***, wykonaj poniższe czynności.

> [!TIP]
> Możesz również pobrać i uruchomić [asystenta odzyskiwania i pomocy technicznej firmy Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) w celu zainstalowania aplikacji Microsoft 365 Apps dla przedsiębiorstw w trybie aktywacji komputerów współużytkowanych.
  
1. Sprawdź posiadaną subskrypcję Microsoft 365. [Dowiedz się, jak](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Jeśli to konieczne, przejdź do innej subskrypcji produktu Microsoft 365. [Dowiedz się, jak](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jeśli pakiet Office jest już zainstalowany na serwerze RDS przy użyciu innych subskrypcji programu Microsoft 365, odinstaluj go. Na przykład, przechodząc do panelu sterowania, \> Odinstaluj program. Odinstaluj za pomocą [asystenta odzyskiwania i pomocy technicznej firmy Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) , jeśli występują problemy.

4. Na serwerze RDS Zaloguj się do centrum administracyjnego usługi Microsoft 365 przy użyciu konta administratora i [Zainstaluj aplikację Microsoft 365 Apps dla przedsiębiorstw](https://portal.office.com/OLS/MySoftware.aspx).

5. Po zainstalowaniu pakietu Office ***nie otwieraj ani nie loguj*** się do żadnych aplikacji pakietu Office.

6. Na serwerze RDS Włącz aktywację komputera udostępnionego, edytując rejestr, wykonując następujące czynności:

1. Kliknij prawym przyciskiem myszy przycisk systemu Windows w lewym dolnym rogu ekranu i wybierz polecenie Uruchom. W polu Otwórz wpisz ciąg **regedit**, a następnie wybierz przycisk OK.

2. Wybierz pozycję tak, gdy zostanie wyświetlony monit o zezwolenie na wprowadzanie zmian na urządzeniu przez Edytor rejestru.

3. W Edytorze rejestru Dodaj wartość ciągu **SharedComputerLicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Na serwerze RDS ***Zaloguj się jako użytkownik końcowy*** i [upewnij się, że Aktywacja komputera udostępnionego jest włączona dla aplikacji Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Aby uzyskać więcej szczegółowych informacji na temat wymagań wstępnych, instrukcji dotyczących konfiguracji i wskazówek dotyczących instalacji niestandardowych przy użyciu narzędzia wdrażania pakietu Office, zobacz [wdrażanie aplikacji Microsoft 365 dla przedsiębiorstw za pomocą usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Aby naprawić błędy związane z aktywacją komputera współużytkowanego, zobacz [Rozwiązywanie problemów z aktywacją komputera w aplikacji Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  
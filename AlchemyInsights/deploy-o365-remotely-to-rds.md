---
title: Wdrażanie Aplikacje Microsoft 365 do użytku udostępnionego w rds, serwerze terminali lub VDI
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077260"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Wdrażanie Aplikacje Microsoft 365 do użytku udostępnionego w rds, serwerze terminali lub VDI

Aby wdrożyć Aplikacje Microsoft 365 usług pulpitu zdalnego (RDS), wcześniej usług terminalowych, należy:

- Użyj łatwej poprawki, aby włączyć standard TLS 1.2 jako domyślny, jeśli korzystasz ze starszej wersji programu Windows (na przykład Windows 7 z dodatkiem SP1 lub Windows Server 2008 R2). Aby uzyskać łatwą poprawkę i uzyskać więcej informacji, zobacz Aktualizowanie w celu włączenia [protokołów TLS 1.1 i TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)jako domyślnych protokołów bezpiecznego w winieHTTP w Windows. 
- Masz plan, który obejmuje Aplikacje Microsoft 365 dla przedsiębiorstw (wcześniej Office 365 Plus). Może to być na przykład Office 365 E3 lub Microsoft 365 E5 albo dowolny plan, który zawiera wersję komputerową programu Project lub Visio, taką jak Project (plan 3) lub Visio (plan 2), albo plan usługi Microsoft 365 Business Premium, który również zawiera Aplikacje Microsoft 365 dla firm.
- Włącz aktywację na komputerze udostępnionym. Aby uzyskać więcej informacji, zobacz Omówienie aktywacji na [komputerze udostępnionym dla użytkowników Aplikacje Microsoft 365.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Uwaga:** Aby zainstalować aplikację Aplikacje Microsoft 365 w trybie aktywacji na komputerze udostępnionym, pobierz i uruchom aplikację [Microsoft Asystent odzyskiwania i pomocy technicznej.](https://aka.ms/SaRA_OfficeSCA_M365Portal) Aby uzyskać szczegółowe informacje na temat wymagań wstępnych, instrukcji konfiguracji i wskazówek dotyczących dostosowywania instalacji za pomocą Narzędzia wdrażania Office, zobacz Wdrażanie usługi Aplikacje Microsoft 365 przy użyciu usług pulpitu [zdalnego.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Aby naprawić błędy związane z aktywacją na komputerze udostępnionym, zobacz:

- [Rozwiązywanie problemów z aktywacją komputera udostępnionego na Aplikacje Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Resetowanie stanu aktywacji aplikacji Aplikacje Microsoft 365 dla przedsiębiorstw.](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Jeśli chcesz zainstalować oprogramowanie w Aplikacje Microsoft 365 RDS z centrum administracyjne platformy Microsoft 365, w którym są używane domyślne ustawienia instalacji, wykonaj następujące czynności:

1. Sprawdź, Microsoft 365 masz plan. Aby uzyskać więcej informacji, zobacz [Która subskrypcja jest posiadana?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. W razie potrzeby zmień plan na Microsoft 365. Aby uzyskać więcej informacji, [zobacz Uaktualnianie do innego planu.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Jeśli Aplikacje Microsoft 365 na serwerze RDS przy użyciu innych niezgodnych planów, odinstaluj go, przechodząc do tematu Odinstalowywanie programu w **Panelu**  >  **sterowania.** W przypadku problemów odinstaluj program, pobierając aplikację [Microsoft Asystent odzyskiwania i pomocy technicznej.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

1. Na serwerze RDS zaloguj się do serwera usługi centrum administracyjne platformy Microsoft 365 za pomocą konta administratora i zainstaluj go [Office.](https://portal.office.com/OLS/MySoftware.aspx)

   Po Office nie otwieraj żadnych aplikacji ani nie loguj się do Office aplikacji.

1. Na serwerze RDS włącz aktywację komputera udostępnionego, edytując rejestr:

   1. Kliknij prawym przyciskiem myszy Windows kliknij prawym przyciskiem myszy w lewym dolnym rogu ekranu, a następnie wybierz polecenie **Uruchom**. W polu Otwórz wpisz polecenie **regedit**, a następnie kliknij przycisk **OK**.

   1. Po wyświetleniu monitu o umożliwienie Edytorowi rejestru zmiany na urządzeniu wybierz pozycję **Tak.**

   1. W Edytorze rejestru w obszarze HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration dodaj wartość ciągu  współużytkowania licencji z ustawieniem **1** .

1. Na serwerze RDS zaloguj się jako użytkownik końcowy i sprawdź, czy włączono aktywację komputera Aplikacje Microsoft 365. 

   Aby uzyskać szczegółowe informacje, zobacz Sprawdzanie, czy na komputerze [udostępnionym włączono aktywację na Aplikacje Microsoft 365.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)
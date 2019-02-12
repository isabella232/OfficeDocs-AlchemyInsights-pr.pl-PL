---
title: Instalowanie pakietu office na serwerze terminali - bez licencji
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918988"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalowanie pakietu Office na serwerze terminali

Do wdrażania pakietu Office 365 ProPlus na serwerze systemu Windows za pomocą usług pulpitu zdalnego (RDS), dawniej usług terminalowych:
  
- Musi mieć plan Office 365, który uwzględnia Office 365 ProPlus, takich jak Office 365 Enterprise E3 lub Enterprise E5. Nie obejmują Office 365 ProPlus planów Office 365 Business i Office 365 Business Premium.
    
- Musisz włączyć [aktywacją udostępnionego komputera](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Jeśli chcesz zainstalować Office 365 ProPlus na licencji RDS z portalu Office 365 ** *który używa domyślnych ustawień instalacji* **, wykonaj następujące kroki: 
  
1. Sprawdź, jaki masz plan Office 365. [Dowiedz się, jak](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Jeśli jest planowane konieczne, przełącz się do innej usługi Office 365. [Dowiedz się, jak](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Jeśli pakiet Office jest już zainstalowany na serwerze usług pulpitu zdalnego za pomocą innych planów usługi Office 365, należy go odinstalować. Na przykład, przechodząc do panelu sterowania \> Odinstalowywanie programu. Należy odinstalować, przy użyciu [pomocy technicznej firmy Microsoft i Asystenta](https://aka.ms/SARA-OfficeUninstall-Alchemy) , jeśli pracujesz w kwestii. 
    
4. Na serwerze usług pulpitu zdalnego należy zalogować się do portalu Office 365 z konta administratora i [zainstalować Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Po zainstalowaniu pakietu Office ** *nie otwieraj ani Zaloguj* ** do dowolnych aplikacji pakietu Office. 
    
6. Na serwerze usług pulpitu zdalnego Włącz aktywację udostępnionego komputera przez edycję rejestru, wykonaj następujące czynności:
    
1. Kliknij prawym przyciskiem myszy przycisk okna w lewym dolnym rogu ekranu, a następnie wybierz polecenie Uruchom. W polu Otwórz wpisz **regedit**, a następnie wybierz przycisk OK. 
    
2. Wybierz tak, gdy pojawi się monit, aby umożliwić Edytora rejestru dokonywać zmian w urządzeniu.
    
3. W Edytorze rejestru, Dodaj wartość ciągu **SharedComputerLicensing** o ustawienie 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. Na serwerze usług pulpitu zdalnego ** *Zaloguj się jako użytkownik końcowy* ** i [Sprawdź, czy aktywacją udostępnionego komputera jest włączone dla Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Aby uzyskać więcej informacji dotyczących wymagań wstępnych, Instalator instrukcje i wytyczne na dostosowanej instalacji przy użyciu narzędzia do wdrażania pakietu Office zobacz [Wdrażanie pakietu Office 365 ProPlus za pomocą usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Aby naprawić błędy związane z aktywacją udostępnionego komputera, zobacz [Rozwiązywanie problemów z aktywacją udostępnionego komputera pakietu Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  


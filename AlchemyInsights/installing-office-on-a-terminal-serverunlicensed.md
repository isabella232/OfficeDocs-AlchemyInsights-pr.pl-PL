---
title: Instalowanie pakietu office na serwerze terminali - bez licencji
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482979"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="dd13d-102">Instalowanie pakietu Office na serwerze terminali</span><span class="sxs-lookup"><span data-stu-id="dd13d-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="dd13d-103">Do wdrażania pakietu Office 365 ProPlus na serwerze systemu Windows za pomocą usług pulpitu zdalnego (RDS), dawniej usług terminalowych:</span><span class="sxs-lookup"><span data-stu-id="dd13d-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="dd13d-p101">Musi mieć plan Office 365, który uwzględnia Office 365 ProPlus, takich jak Office 365 Enterprise E3 lub Enterprise E5. Nie obejmują Office 365 ProPlus planów Office 365 Business i Office 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="dd13d-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="dd13d-106">Musisz włączyć [aktywacją udostępnionego komputera](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="dd13d-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="dd13d-107">Jeśli chcesz zainstalować Office 365 ProPlus na licencji RDS z portalu Office 365 \*\* *który używa domyślnych ustawień instalacji* \*\*, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="dd13d-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="dd13d-p102">Sprawdź, jaki masz plan Office 365. [Dowiedz się, jak](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="dd13d-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="dd13d-p103">Jeśli jest planowane konieczne, przełącz się do innej usługi Office 365. [Dowiedz się, jak](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="dd13d-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="dd13d-p104">Jeśli pakiet Office jest już zainstalowany na serwerze usług pulpitu zdalnego za pomocą innych planów usługi Office 365, należy go odinstalować. Na przykład, przechodząc do panelu sterowania \> Odinstalowywanie programu. Należy odinstalować, przy użyciu [pomocy technicznej firmy Microsoft i Asystenta](https://aka.ms/SARA-OfficeUninstall-Alchemy) , jeśli pracujesz w kwestii.</span><span class="sxs-lookup"><span data-stu-id="dd13d-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="dd13d-115">Na serwerze usług pulpitu zdalnego należy zalogować się do portalu Office 365 z konta administratora i [zainstalować Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="dd13d-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="dd13d-116">Po zainstalowaniu pakietu Office \*\* *nie otwieraj ani Zaloguj* \*\* do dowolnych aplikacji pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="dd13d-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="dd13d-117">Na serwerze usług pulpitu zdalnego Włącz aktywację udostępnionego komputera przez edycję rejestru, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="dd13d-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="dd13d-p105">Kliknij prawym przyciskiem myszy przycisk okna w lewym dolnym rogu ekranu, a następnie wybierz polecenie Uruchom. W polu Otwórz wpisz **regedit**, a następnie wybierz przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="dd13d-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="dd13d-120">Wybierz tak, gdy pojawi się monit, aby umożliwić Edytora rejestru dokonywać zmian w urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="dd13d-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="dd13d-121">W Edytorze rejestru, Dodaj wartość ciągu **SharedComputerLicensing** o ustawienie 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="dd13d-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="dd13d-122">Na serwerze usług pulpitu zdalnego \*\* *Zaloguj się jako użytkownik końcowy* \*\* i [Sprawdź, czy aktywacją udostępnionego komputera jest włączone dla Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="dd13d-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="dd13d-123">Aby uzyskać więcej informacji dotyczących wymagań wstępnych, Instalator instrukcje i wytyczne na dostosowanej instalacji przy użyciu narzędzia do wdrażania pakietu Office zobacz [Wdrażanie pakietu Office 365 ProPlus za pomocą usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="dd13d-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="dd13d-124">Aby naprawić błędy związane z aktywacją udostępnionego komputera, zobacz [Rozwiązywanie problemów z aktywacją udostępnionego komputera pakietu Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="dd13d-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  


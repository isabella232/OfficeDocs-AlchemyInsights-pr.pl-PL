---
title: Instalowanie pakietu Office na serwerze terminali — bez licencji
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735399"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="b8dd7-102">Instalowanie pakietu Office na serwerze terminali</span><span class="sxs-lookup"><span data-stu-id="b8dd7-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="b8dd7-103">Aby wdrożyć pakiet Office 365 ProPlus w systemie Windows Server przy użyciu usług pulpitu zdalnego (RDS), dawniej nazywanych usługami terminalowymi:</span><span class="sxs-lookup"><span data-stu-id="b8dd7-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="b8dd7-104">Musi mieć plan 365 pakietu Office, który zawiera pakiet Office 365 ProPlus, takich jak Office 365 Enterprise E3 lub Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="b8dd7-105">Plany Office 365 Business i Office 365 Business Premium nie zawierają pakietu Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="b8dd7-106">Należy włączyć [aktywację udostępnionego komputera](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="b8dd7-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="b8dd7-107">Jeśli chcesz zainstalować pakiet Office 365 ProPlus na RDS z centrum administracyjnego Microsoft 365, ***który używa domyślnych ustawień instalacji***, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="b8dd7-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="b8dd7-108">Sprawdź, co masz plan 365 Office.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="b8dd7-109">Dowiedz się, jak</span><span class="sxs-lookup"><span data-stu-id="b8dd7-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="b8dd7-110">Jeśli to konieczne, przełącz się do innego pakietu Office 365 plan.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="b8dd7-111">Dowiedz się, jak</span><span class="sxs-lookup"><span data-stu-id="b8dd7-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="b8dd7-112">Jeśli pakiet Office jest już zainstalowany na serwerze usług pulpitu zdalnego przy użyciu innych planów pakietu Office 365, odinstaluj go.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="b8dd7-113">Na przykład, przechodząc do panelu \> sterowania Odinstaluj program.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="b8dd7-114">Odinstaluj, korzystając z [pomocy technicznej firmy Microsoft i asystenta odzyskiwania](https://aka.ms/SARA-OfficeUninstall-Alchemy) , jeśli masz problemy z uruchamianiem.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="b8dd7-115">Na serwerze RDS Zaloguj się do centrum administracyjnego Microsoft 365 z kontem administratora i [Zainstaluj pakiet Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="b8dd7-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="b8dd7-116">Po zainstalowaniu pakietu Office ***nie otwieraj ani nie logujesz*** się do żadnych aplikacji pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="b8dd7-117">Na serwerze usług pulpitu zdalnego Włącz aktywację udostępnionego komputera, edytując rejestr, wykonując następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="b8dd7-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="b8dd7-118">Kliknij prawym przyciskiem myszy przycisk Windows w lewym dolnym rogu ekranu i wybierz polecenie Uruchom.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="b8dd7-119">W polu Otwórz wpisz **regedit**, a następnie wybierz przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="b8dd7-120">Wybierz opcję tak po wyświetleniu monitu, aby zezwolić edytorowi rejestru na wprowadzanie zmian w urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="b8dd7-121">W Edytorze rejestru Dodaj wartość ciągu **Sharedcomputerlicensing** z ustawieniem 1 pod HKEY_LOCAL_MACHINE\Software\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="b8dd7-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="b8dd7-122">Na serwerze usług pulpitu zdalnego ***Zaloguj się jako użytkownik końcowy*** i [Sprawdź, czy aktywacja udostępnionego komputera jest włączona dla pakietu Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="b8dd7-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="b8dd7-123">Aby uzyskać więcej informacji na temat wymagań wstępnych, instrukcje instalacji i wskazówki dotyczące instalacji dostosowanych za pomocą narzędzia wdrażania pakietu Office, zobacz [wdrażanie pakietu office 365 ProPlus przy użyciu usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="b8dd7-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="b8dd7-124">Aby naprawić błędy związane z aktywacją komputera udostępnionego, zobacz [Rozwiązywanie problemów z aktywacją komputera udostępnionego dla pakietu Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="b8dd7-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  
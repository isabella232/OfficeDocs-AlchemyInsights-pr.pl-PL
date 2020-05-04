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
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010624"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="8d4c9-102">Instalowanie pakietu Office na serwerze terminali</span><span class="sxs-lookup"><span data-stu-id="8d4c9-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="8d4c9-103">Aby wdrożyć aplikacje usługi Microsoft 365 dla przedsiębiorstw w systemie Windows Server przy użyciu usług pulpitu zdalnego (RDS), wcześniej nazwanych usługami terminalowymi:</span><span class="sxs-lookup"><span data-stu-id="8d4c9-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="8d4c9-104">Musisz mieć subskrypcję usługi Microsoft 365, która obejmuje aplikacje microsoft 365 dla przedsiębiorstw, takie jak Office 365 Enterprise E3 lub Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="8d4c9-105">Plany microsoft 365 Apps dla firm i Microsoft 365 Apps for business Premium nie obejmują aplikacji Microsoft 365 dla przedsiębiorstw.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="8d4c9-106">Należy włączyć [aktywację komputera współdzielonego](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="8d4c9-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="8d4c9-107">Jeśli chcesz zainstalować usługę Microsoft 365 Apps dla przedsiębiorstw na usługach RDS z centrum administracyjnego usługi Microsoft 365, ***które używa domyślnych ustawień instalacji,*** należy wykonać następujące czynności.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="8d4c9-108">Można również pobrać i uruchomić [Asystenta pomocy technicznej i odzyskiwania firmy Microsoft,](https://aka.ms/SaRA_OfficeSCA_M365Portal) aby zainstalować aplikacje microsoft 365 dla przedsiębiorstwa w trybie aktywacji komputera udostępnionego.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="8d4c9-109">Sprawdź, jaką masz subskrypcję usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="8d4c9-110">Dowiedz się, jak</span><span class="sxs-lookup"><span data-stu-id="8d4c9-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="8d4c9-111">W razie potrzeby przełącz się na inną subskrypcję usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="8d4c9-112">Dowiedz się, jak</span><span class="sxs-lookup"><span data-stu-id="8d4c9-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="8d4c9-113">Jeśli pakiet Office jest już zainstalowany na serwerze usług pulpitu zdalnego przy użyciu innych subskrypcji usługi Microsoft 365, odinstaluj go.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="8d4c9-114">Na przykład, przechodząc do \> Panelu sterowania Odinstaluj program.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="8d4c9-115">Odinstaluj za pomocą [Pomocy technicznej firmy Microsoft i Asystenta odzyskiwania,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jeśli występują problemy.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="8d4c9-116">Na serwerze usług pulpitu zdalnego zaloguj się do centrum administracyjnego usługi Microsoft 365 za pomocą konta administratora i [zainstaluj aplikację Microsoft 365 Apps dla przedsiębiorstw](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="8d4c9-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="8d4c9-117">Po zainstalowaniu pakietu Office ***nie otwieraj ani nie loguj*** się do żadnych aplikacji pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="8d4c9-118">Na serwerze usług pulpitu zdalnego włącz aktywację komputera udostępnionego, edytując rejestr, wykonując następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="8d4c9-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="8d4c9-119">Kliknij prawym przyciskiem myszy przycisk Windows w lewym dolnym rogu ekranu i wybierz pozycję Uruchom.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="8d4c9-120">W polu Otwórz wpisz **regedit**, a następnie wybierz przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="8d4c9-121">Wybierz pozycję Tak po wyświetleniu monitu, aby zezwolić Edytorowi rejestru na wprowadzanie zmian na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="8d4c9-122">W Edytorze rejestru dodaj wartość ciągu **SharedComputerLicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="8d4c9-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="8d4c9-123">Na serwerze usług pulpitu ***zdalnego zaloguj się jako użytkownik końcowy*** i [sprawdź, czy aktywacja udostępnionego komputera jest włączona dla aplikacji usługi Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="8d4c9-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="8d4c9-124">Aby uzyskać więcej informacji na temat wymagań wstępnych, instrukcji konfiguracji i wskazówek dotyczących niestandardowych instalacji przy użyciu Narzędzia wdrażania pakietu Office, zobacz [Wdrażanie aplikacji microsoft 365 dla przedsiębiorstw przy użyciu usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="8d4c9-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="8d4c9-125">Aby naprawić błędy związane z aktywacją komputera współdzielonego, zobacz [Rozwiązywanie problemów z aktywacją komputera udostępnionego dla aplikacji usługi Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="8d4c9-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  
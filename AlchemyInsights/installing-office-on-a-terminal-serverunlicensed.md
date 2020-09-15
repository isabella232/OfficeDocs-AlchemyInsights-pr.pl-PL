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
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="2e91c-102">Instalowanie pakietu Office na serwerze terminali</span><span class="sxs-lookup"><span data-stu-id="2e91c-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="2e91c-103">Wdrażanie aplikacji Microsoft 365 dla przedsiębiorstw na serwerze z systemem Windows przy użyciu usług pulpitu zdalnego (RDS) — dawniej nazywane usługami terminalowymi:</span><span class="sxs-lookup"><span data-stu-id="2e91c-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="2e91c-104">Musisz mieć subskrypcję programu Microsoft 365 obejmującą aplikacje Microsoft 365 dla przedsiębiorstw, takie jak Office 365 Enterprise E3 lub Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="2e91c-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="2e91c-105">Pakiet Microsoft 365 Apps dla firm i aplikacje Microsoft 365 dla firm w wersji Premium nie zawierają aplikacji Microsoft 365 Apps dla przedsiębiorstw.</span><span class="sxs-lookup"><span data-stu-id="2e91c-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="2e91c-106">Musisz włączyć [aktywację komputera współużytkowanego](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="2e91c-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="2e91c-107">Jeśli chcesz zainstalować aplikacje Microsoft 365 dla przedsiębiorstw na komputerze RDS z centrum administracyjnego Microsoft 365, ***które korzysta z domyślnych ustawień instalacji***, wykonaj poniższe czynności.</span><span class="sxs-lookup"><span data-stu-id="2e91c-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="2e91c-108">Możesz również pobrać i uruchomić [asystenta odzyskiwania i pomocy technicznej firmy Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) w celu zainstalowania aplikacji Microsoft 365 Apps dla przedsiębiorstw w trybie aktywacji komputerów współużytkowanych.</span><span class="sxs-lookup"><span data-stu-id="2e91c-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="2e91c-109">Sprawdź posiadaną subskrypcję Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2e91c-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="2e91c-110">Dowiedz się, jak</span><span class="sxs-lookup"><span data-stu-id="2e91c-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="2e91c-111">Jeśli to konieczne, przejdź do innej subskrypcji produktu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2e91c-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="2e91c-112">Dowiedz się, jak</span><span class="sxs-lookup"><span data-stu-id="2e91c-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="2e91c-113">Jeśli pakiet Office jest już zainstalowany na serwerze RDS przy użyciu innych subskrypcji programu Microsoft 365, odinstaluj go.</span><span class="sxs-lookup"><span data-stu-id="2e91c-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="2e91c-114">Na przykład, przechodząc do panelu sterowania, \> Odinstaluj program.</span><span class="sxs-lookup"><span data-stu-id="2e91c-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="2e91c-115">Odinstaluj za pomocą [asystenta odzyskiwania i pomocy technicznej firmy Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) , jeśli występują problemy.</span><span class="sxs-lookup"><span data-stu-id="2e91c-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="2e91c-116">Na serwerze RDS Zaloguj się do centrum administracyjnego usługi Microsoft 365 przy użyciu konta administratora i [Zainstaluj aplikację Microsoft 365 Apps dla przedsiębiorstw](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="2e91c-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="2e91c-117">Po zainstalowaniu pakietu Office ***nie otwieraj ani nie loguj*** się do żadnych aplikacji pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="2e91c-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="2e91c-118">Na serwerze RDS Włącz aktywację komputera udostępnionego, edytując rejestr, wykonując następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="2e91c-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="2e91c-119">Kliknij prawym przyciskiem myszy przycisk systemu Windows w lewym dolnym rogu ekranu i wybierz polecenie Uruchom.</span><span class="sxs-lookup"><span data-stu-id="2e91c-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="2e91c-120">W polu Otwórz wpisz ciąg **regedit**, a następnie wybierz przycisk OK.</span><span class="sxs-lookup"><span data-stu-id="2e91c-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="2e91c-121">Wybierz pozycję tak, gdy zostanie wyświetlony monit o zezwolenie na wprowadzanie zmian na urządzeniu przez Edytor rejestru.</span><span class="sxs-lookup"><span data-stu-id="2e91c-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="2e91c-122">W Edytorze rejestru Dodaj wartość ciągu **SharedComputerLicensing** z ustawieniem 1 w obszarze HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="2e91c-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="2e91c-123">Na serwerze RDS ***Zaloguj się jako użytkownik końcowy*** i [upewnij się, że Aktywacja komputera udostępnionego jest włączona dla aplikacji Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="2e91c-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="2e91c-124">Aby uzyskać więcej szczegółowych informacji na temat wymagań wstępnych, instrukcji dotyczących konfiguracji i wskazówek dotyczących instalacji niestandardowych przy użyciu narzędzia wdrażania pakietu Office, zobacz [wdrażanie aplikacji Microsoft 365 dla przedsiębiorstw za pomocą usług pulpitu zdalnego](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="2e91c-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="2e91c-125">Aby naprawić błędy związane z aktywacją komputera współużytkowanego, zobacz [Rozwiązywanie problemów z aktywacją komputera w aplikacji Microsoft 365 dla przedsiębiorstw](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="2e91c-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  
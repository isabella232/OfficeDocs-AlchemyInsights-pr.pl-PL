---
title: Korzystanie z narzędzia wdrażania pakietu Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726258"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="ba9bd-102">Korzystanie z narzędzia wdrażania pakietu Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="ba9bd-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="ba9bd-103">Narzędzie wdrażania pakietu Office (ODT) służy do wdrażania wersji pakietu Office 365 pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ba9bd-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="ba9bd-104">Narzędzie wdrażania pakietu Office (setup.exe) jest uruchamiane z wiersza polecenia i używa konfiguracyjnego pliku XML do określenia, jakie ustawienia należy zastosować podczas wdrażania pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ba9bd-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="ba9bd-105">Pobierz najnowszą wersję narzędzia wdrażania pakietu Office z [Centrum pobierania Firmy Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="ba9bd-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="ba9bd-106">Użyj [narzędzia dostosowywania pakietu Office (OCT),](https://config.office.com) aby wybrać preferencje wdrażania i utworzyć plik XML konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="ba9bd-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="ba9bd-107">Wyeksportuj plik konfiguracyjny i umieść go lokalnie w tym samym folderze, w którym znajduje się plik setup.exe.</span><span class="sxs-lookup"><span data-stu-id="ba9bd-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="ba9bd-108">**Uwaga:** Często występują problemy z instalacją pakietu Office z powodu nieprawidłowo skonfigurowanych lub nieprawidłowo sformatowanych plików konfiguracyjnych.</span><span class="sxs-lookup"><span data-stu-id="ba9bd-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="ba9bd-109">Aby uniknąć takich problemów, zaleca się użycie narzędzia dostosowywania pakietu Office do utworzenia pliku konfiguracyjnego.</span><span class="sxs-lookup"><span data-stu-id="ba9bd-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="ba9bd-110">Istniejące pliki konfiguracyjne można również zaimportować do narzędzia dostosowywania pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ba9bd-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="ba9bd-111">W wierszu polecenia z podwyższonym poziomem uprawnień przełącz się do lokalizacji, w której znajduje się plik setup.exe, i uruchom Narzędzie wdrażania pakietu Office w trybie pobierania i określ właśnie zapisany plik konfiguracyjny.</span><span class="sxs-lookup"><span data-stu-id="ba9bd-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="ba9bd-112">W tym przykładzie plik konfiguracyjny nosi nazwę Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="ba9bd-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="ba9bd-113">Uruchom Narzędzie wdrażania pakietu Office w trybie konfiguracji i określ plik konfiguracyjny.</span><span class="sxs-lookup"><span data-stu-id="ba9bd-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="ba9bd-114">**Uwaga:** Ten krok należy uruchomić z komputera klienckiego, na którym ma zostać zainstalowany pakiet Office, i musi mieć uprawnienia administratora lokalnego na tym komputerze.</span><span class="sxs-lookup"><span data-stu-id="ba9bd-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="ba9bd-115">Aby dowiedzieć się więcej na temat korzystania z Narzędzia wdrażania pakietu Office dla aplikacji usługi Microsoft 365 w scenariuszach wdrażania w przedsiębiorstwie, zobacz [Omówienie Narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="ba9bd-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="ba9bd-116">Aby uzyskać więcej informacji na temat korzystania z narzędzia dostosowywania pakietu Office, zobacz [Omówienie narzędzia dostosowywania pakietu Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="ba9bd-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>

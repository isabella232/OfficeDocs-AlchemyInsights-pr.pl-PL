---
title: Za pomocą narzędzia wdrażania pakietu Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365535"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="ad07b-102">Przy użyciu narzędzia do wdrażania pakietu Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="ad07b-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="ad07b-103">Narzędzie wdrażania pakietu Office (ODT) umożliwia wdrażanie wersji Office 365 pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ad07b-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="ad07b-104">Narzędzia do wdrażania pakietu Office (setup.exe) jest uruchamiany z wiersza polecenia i używa pliku XML konfiguracji ustalenie, jakie ustawienia mają zastosowanie podczas wdrażania pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ad07b-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="ad07b-105">Pobierz najnowszą wersję narzędzia wdrażania pakietu Office z witryny [Microsoft — Centrum pobierania](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="ad07b-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="ad07b-106">Użyj [Narzędzia dostosowywania pakietu Office (OCT)](https://config.office.com) , aby wybrać preferencji dotyczących wdrożenia i utworzyć plik konfiguracji XML.</span><span class="sxs-lookup"><span data-stu-id="ad07b-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="ad07b-107">Wyeksportować plik konfiguracyjny i umieść go lokalnie na tym samym folderze, w którym znajduje się setup.exe.</span><span class="sxs-lookup"><span data-stu-id="ad07b-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="ad07b-108">**Uwaga:** Instalacja pakietu Office, które często występują problemy ze względu na niepoprawnie skonfigurowany lub malformatted plików konfiguracyjnych.</span><span class="sxs-lookup"><span data-stu-id="ad07b-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="ad07b-109">Aby uniknąć takich problemów, zaleca się użyć narzędzia dostosowywania pakietu Office do tworzenia pliku konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="ad07b-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="ad07b-110">Można także importować istniejące pliki konfiguracyjne do narzędzia dostosowywania pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ad07b-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="ad07b-111">Z wiersza polecenia Przełącz się do lokalizacji, gdzie znajduje się setup.exe i uruchom narzędzie wdrażania pakietu Office w trybie pobierania i określ plik konfiguracji, który został zapisany.</span><span class="sxs-lookup"><span data-stu-id="ad07b-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="ad07b-112">W tym przykładzie plik konfiguracyjny o nazwie Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="ad07b-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="ad07b-113">Uruchom Narzędzie wdrażania pakietu Office w trybie skonfigurować i określić plik konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="ad07b-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="ad07b-114">**Uwaga:** W tym kroku należy uruchomić z komputera klienckiego, na którym chcesz zainstalować pakiet Office i musi mieć uprawnienia administratora lokalnego na tym komputerze.</span><span class="sxs-lookup"><span data-stu-id="ad07b-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="ad07b-115">Aby dowiedzieć się więcej na temat używania narzędzia wdrażania pakietu Office Office 365 ProPlus scenariuszy wdrażania, zobacz [Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="ad07b-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="ad07b-116">Aby uzyskać więcej informacji dotyczących sposobu używania narzędzia dostosowywania pakietu Office zobacz [Omówienie narzędzia dostosowywania pakietu Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="ad07b-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>

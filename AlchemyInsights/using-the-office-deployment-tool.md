---
title: Za pomocą narzędzia wdrażania pakietu Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482705"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="04756-102">Przy użyciu narzędzia do wdrażania pakietu Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="04756-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="04756-p101">Narzędzie wdrażania pakietu Office (ODT) umożliwia wdrażanie wersji Office 365 pakietu Office. Narzędzia do wdrażania pakietu Office (setup.exe) jest uruchamiany z wiersza polecenia i używa pliku XML konfiguracji ustalenie, jakie ustawienia mają zastosowanie podczas wdrażania pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="04756-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="04756-105">Pobierz najnowszą wersję narzędzia wdrażania pakietu Office z witryny [Microsoft — Centrum pobierania](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="04756-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="04756-p102">Użyj [Narzędzia dostosowywania pakietu Office (OCT)](https://config.office.com) , aby wybrać preferencji dotyczących wdrożenia i utworzyć plik konfiguracji XML. Wyeksportować plik konfiguracyjny i umieść go lokalnie na tym samym folderze, w którym znajduje się setup.exe.</span><span class="sxs-lookup"><span data-stu-id="04756-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="04756-p103">**Uwaga:** Instalacja pakietu Office, które często występują problemy ze względu na niepoprawnie skonfigurowany lub malformatted plików konfiguracyjnych. Aby uniknąć takich problemów, zaleca się użyć narzędzia dostosowywania pakietu Office do tworzenia pliku konfiguracji. Można także importować istniejące pliki konfiguracyjne do narzędzia dostosowywania pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="04756-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="04756-p104">Z wiersza polecenia Przełącz się do lokalizacji, gdzie znajduje się setup.exe i uruchom narzędzie wdrażania pakietu Office w trybie pobierania i określ plik konfiguracji, który został zapisany. W tym przykładzie plik konfiguracyjny o nazwie Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="04756-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="04756-113">Uruchom Narzędzie wdrażania pakietu Office w trybie skonfigurować i określić plik konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="04756-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="04756-114">**Uwaga:** W tym kroku należy uruchomić z komputera klienckiego, na którym chcesz zainstalować pakiet Office i musi mieć uprawnienia administratora lokalnego na tym komputerze.</span><span class="sxs-lookup"><span data-stu-id="04756-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="04756-p105">Aby dowiedzieć się więcej na temat używania narzędzia wdrażania pakietu Office Office 365 ProPlus scenariuszy wdrażania, zobacz [Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Aby uzyskać więcej informacji dotyczących sposobu używania narzędzia dostosowywania pakietu Office zobacz [Omówienie narzędzia dostosowywania pakietu Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="04756-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  


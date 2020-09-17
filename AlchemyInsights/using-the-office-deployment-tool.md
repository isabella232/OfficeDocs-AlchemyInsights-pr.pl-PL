---
title: Korzystanie z narzędzia wdrażania pakietu Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794921"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="2224d-102">Korzystanie z narzędzia wdrażania pakietu Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="2224d-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="2224d-103">Aby wdrożyć pakiet Office 365, użyj narzędzia wdrażania pakietu Office (ODT).</span><span class="sxs-lookup"><span data-stu-id="2224d-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="2224d-104">Narzędzie wdrażania pakietu Office (setup.exe) jest uruchamiane z wiersza polecenia i używa pliku XML konfiguracji w celu określenia ustawień, które mają zostać zastosowane podczas wdrażania pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="2224d-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="2224d-105">Pobierz najnowszą wersję narzędzia wdrażania pakietu Office z [Centrum pobierania Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="2224d-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="2224d-106">Za pomocą [narzędzia dostosowywania pakietu Office (KTZ)](https://config.office.com) wybierz Preferencje wdrażania i Utwórz plik XML konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="2224d-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="2224d-107">Wyeksportuj plik konfiguracji i umieść go lokalnie w tym samym folderze, w którym znajduje się setup.exe.</span><span class="sxs-lookup"><span data-stu-id="2224d-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="2224d-108">**Uwaga:** Problemy z instalacją pakietu Office występują często wskutek błędnie skonfigurowanych lub malformatted plików konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="2224d-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="2224d-109">Aby uniknąć takich problemów, zalecamy utworzenie pliku konfiguracji za pomocą narzędzia dostosowywania pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="2224d-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="2224d-110">Możesz również zaimportować istniejące pliki konfiguracyjne do narzędzia dostosowywania pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="2224d-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="2224d-111">W wierszu polecenia z podwyższonym poziomem uprawnień przejdź do lokalizacji, w której setup.exe się znajdować, i uruchom narzędzie wdrażania pakietu Office w trybie pobierania i określ plik konfiguracji, który właśnie został zapisany.</span><span class="sxs-lookup"><span data-stu-id="2224d-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="2224d-112">W tym przykładzie plik konfiguracji ma nazwę Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="2224d-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setup.exe /download Configuration.xml```

<span data-ttu-id="2224d-113">4. Uruchom narzędzie wdrażania pakietu Office w trybie konfiguracji i określ plik konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="2224d-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setup.exe /configure Configuration.xml```

<span data-ttu-id="2224d-114">**Uwaga:** Musisz uruchomić ten krok z komputera klienckiego, na którym chcesz zainstalować pakiet Office, i musisz mieć lokalne uprawnienia administratora na tym komputerze.</span><span class="sxs-lookup"><span data-stu-id="2224d-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="2224d-115">Aby dowiedzieć się więcej na temat korzystania z narzędzia wdrażania pakietu Office dla scenariuszy wdrażania aplikacji Microsoft 365 dla firm, zobacz [Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="2224d-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="2224d-116">Aby uzyskać więcej informacji na temat korzystania z narzędzia dostosowywania pakietu Office, zobacz [Omówienie narzędzia do dostosowywania pakietu Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="2224d-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>

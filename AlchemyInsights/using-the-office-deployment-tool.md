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
# <a name="using-the-office-deployment-tool-odt"></a>Korzystanie z narzędzia wdrażania pakietu Office (ODT)

Aby wdrożyć pakiet Office 365, użyj narzędzia wdrażania pakietu Office (ODT). Narzędzie wdrażania pakietu Office (setup.exe) jest uruchamiane z wiersza polecenia i używa pliku XML konfiguracji w celu określenia ustawień, które mają zostać zastosowane podczas wdrażania pakietu Office.
  
1. Pobierz najnowszą wersję narzędzia wdrażania pakietu Office z [Centrum pobierania Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Za pomocą [narzędzia dostosowywania pakietu Office (KTZ)](https://config.office.com) wybierz Preferencje wdrażania i Utwórz plik XML konfiguracji. Wyeksportuj plik konfiguracji i umieść go lokalnie w tym samym folderze, w którym znajduje się setup.exe.

    **Uwaga:** Problemy z instalacją pakietu Office występują często wskutek błędnie skonfigurowanych lub malformatted plików konfiguracji. Aby uniknąć takich problemów, zalecamy utworzenie pliku konfiguracji za pomocą narzędzia dostosowywania pakietu Office. Możesz również zaimportować istniejące pliki konfiguracyjne do narzędzia dostosowywania pakietu Office.

3. W wierszu polecenia z podwyższonym poziomem uprawnień przejdź do lokalizacji, w której setup.exe się znajdować, i uruchom narzędzie wdrażania pakietu Office w trybie pobierania i określ plik konfiguracji, który właśnie został zapisany. W tym przykładzie plik konfiguracji ma nazwę Configuration.xml:

```setup.exe /download Configuration.xml```

4. Uruchom narzędzie wdrażania pakietu Office w trybie konfiguracji i określ plik konfiguracji.

```setup.exe /configure Configuration.xml```

**Uwaga:** Musisz uruchomić ten krok z komputera klienckiego, na którym chcesz zainstalować pakiet Office, i musisz mieć lokalne uprawnienia administratora na tym komputerze.

Aby dowiedzieć się więcej na temat korzystania z narzędzia wdrażania pakietu Office dla scenariuszy wdrażania aplikacji Microsoft 365 dla firm, zobacz [Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Aby uzyskać więcej informacji na temat korzystania z narzędzia dostosowywania pakietu Office, zobacz [Omówienie narzędzia do dostosowywania pakietu Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).

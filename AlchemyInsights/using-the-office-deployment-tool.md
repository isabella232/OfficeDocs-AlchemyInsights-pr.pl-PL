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
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085842"
---
# <a name="using-the-office-deployment-tool-odt"></a>Korzystanie z narzędzia wdrażania pakietu Office (ODT)

Aby wdrożyć pakiet Office 365, użyj narzędzia wdrażania pakietu Office (ODT). Narzędzie wdrażania pakietu Office (setupodt.exe) jest uruchamiane z wiersza polecenia i używa pliku XML konfiguracji w celu określenia ustawień, które mają zostać zastosowane podczas wdrażania pakietu Office.
  
1. Pobierz najnowszą wersję narzędzia wdrażania pakietu Office z [Centrum pobierania Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Za pomocą [narzędzia dostosowywania pakietu Office (KTZ)](https://config.office.com) wybierz Preferencje wdrażania i Utwórz plik XML konfiguracji. Wyeksportuj plik konfiguracji i umieść go lokalnie w tym samym folderze, w którym znajduje się setupodt.exe.

    **Uwaga:** Problemy z instalacją pakietu Office występują często wskutek błędnie skonfigurowanych lub malformatted plików konfiguracji. Aby uniknąć takich problemów, zalecamy utworzenie pliku konfiguracji za pomocą narzędzia dostosowywania pakietu Office. Możesz również zaimportować istniejące pliki konfiguracyjne do narzędzia dostosowywania pakietu Office.

3. W wierszu polecenia z podwyższonym poziomem uprawnień przejdź do lokalizacji, w której setupodt.exe się znajdować, i uruchom narzędzie wdrażania pakietu Office w trybie pobierania i określ plik konfiguracji, który właśnie został zapisany. W tym przykładzie plik konfiguracji ma nazwę Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Uruchom narzędzie wdrażania pakietu Office w trybie konfiguracji i określ plik konfiguracji.

```setupodt.exe /configure Configuration.xml```

**Uwaga:** Musisz uruchomić ten krok z komputera klienckiego, na którym chcesz zainstalować pakiet Office, i musisz mieć lokalne uprawnienia administratora na tym komputerze.

Aby dowiedzieć się więcej na temat korzystania z narzędzia wdrażania pakietu Office dla scenariuszy wdrażania aplikacji Microsoft 365 dla firm, zobacz [Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Aby uzyskać więcej informacji na temat korzystania z narzędzia dostosowywania pakietu Office, zobacz [Omówienie narzędzia do dostosowywania pakietu Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).

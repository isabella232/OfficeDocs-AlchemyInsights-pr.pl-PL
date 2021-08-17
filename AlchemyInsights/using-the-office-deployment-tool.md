---
title: Korzystanie z Office wdrażania
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083780"
---
# <a name="using-the-office-deployment-tool-odt"></a>Korzystanie z narzędzia Office wdrażania (ODT)

Narzędzie wdrażania Office (ODT) umożliwia wdrażanie Office 365 wersji Office. Narzędzie Office wdrażania programu (setup.exe) jest uruchamiane z wiersza polecenia i używa pliku XML konfiguracji w celu określenia, jakie ustawienia mają być stosowane podczas wdrażania Office.
  
1. Pobierz najnowszą wersję narzędzia wdrażania pakietu Office z [Centrum pobierania Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Użyj narzędzia [Office dostosowywania (OCT),](https://config.office.com) aby wybrać preferencje wdrażania i utworzyć plik XML konfiguracji. Wyeksportuj plik konfiguracji i umieść go lokalnie w tym samym folderze, w setup.exe się znajduje.

    **Uwaga:** Office problemy z instalacją występują często z powodu nieprawidłowo skonfigurowanych lub nieprawidłowo sformatowanych plików konfiguracji. Aby uniknąć takich problemów, zalecamy utworzenie pliku konfiguracji Office pomocą narzędzia do dostosowywania ustawień. Możesz również zaimportować istniejące pliki konfiguracji do narzędzia Office dostosowywania.

3. W wierszu polecenia z podwyższonym poziomem uprawnień przejdź do lokalizacjisetup.exe w której się znajduje, uruchom narzędzie wdrażania pakietu Office w trybie pobierania i określ właśnie zapisany plik konfiguracji. W tym przykładzie plik konfiguracji ma nazwę Configuration.xml:

```setup.exe /download Configuration.xml```

4.Uruchom narzędzie Office w trybie konfiguracji i określ plik konfiguracji.

```setup.exe /configure Configuration.xml```

**Uwaga:** Ten krok należy wykonać na komputerze klienckim, na którym chcesz zainstalować pakiet Office i musisz mieć uprawnienia administratora lokalnego na tym komputerze.

Aby dowiedzieć się więcej na temat Office wdrażania na Aplikacje Microsoft 365 dla przedsiębiorstw scenariuszy wdrażania, zobacz Omówienie narzędzia Office [wdrażania.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Aby uzyskać więcej informacji na temat korzystania z narzędzia Office dostosowywania, zobacz Omówienie narzędzia Office [dostosowywania.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)

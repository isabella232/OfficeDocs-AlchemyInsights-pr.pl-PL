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
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010877"
---
# <a name="using-the-office-deployment-tool-odt"></a>Korzystanie z narzędzia wdrażania pakietu Office (ODT)

Narzędzie wdrażania pakietu Office (ODT) służy do wdrażania wersji pakietu Office 365 pakietu Office. Narzędzie wdrażania pakietu Office (setup.exe) jest uruchamiane z wiersza polecenia i używa konfiguracyjnego pliku XML do określenia, jakie ustawienia należy zastosować podczas wdrażania pakietu Office.
  
1. Pobierz najnowszą wersję narzędzia wdrażania pakietu Office z [Centrum pobierania Firmy Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Użyj [narzędzia dostosowywania pakietu Office (OCT),](https://config.office.com) aby wybrać preferencje wdrażania i utworzyć plik XML konfiguracji. Wyeksportuj plik konfiguracyjny i umieść go lokalnie w tym samym folderze, w którym znajduje się plik setup.exe.

    **Uwaga:** Często występują problemy z instalacją pakietu Office z powodu nieprawidłowo skonfigurowanych lub nieprawidłowo sformatowanych plików konfiguracyjnych. Aby uniknąć takich problemów, zaleca się użycie narzędzia dostosowywania pakietu Office do utworzenia pliku konfiguracyjnego. Istniejące pliki konfiguracyjne można również zaimportować do narzędzia dostosowywania pakietu Office.

3. W wierszu polecenia z podwyższonym poziomem uprawnień przełącz się do lokalizacji, w której znajduje się plik setup.exe, i uruchom Narzędzie wdrażania pakietu Office w trybie pobierania i określ właśnie zapisany plik konfiguracyjny. W tym przykładzie plik konfiguracyjny nosi nazwę Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Uruchom Narzędzie wdrażania pakietu Office w trybie konfiguracji i określ plik konfiguracyjny.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Uwaga:** Ten krok należy uruchomić z komputera klienckiego, na którym ma zostać zainstalowany pakiet Office, i musi mieć uprawnienia administratora lokalnego na tym komputerze.

Aby dowiedzieć się więcej na temat korzystania z Narzędzia wdrażania pakietu Office dla aplikacji usługi Microsoft 365 w scenariuszach wdrażania w przedsiębiorstwie, zobacz [Omówienie Narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Aby uzyskać więcej informacji na temat korzystania z narzędzia dostosowywania pakietu Office, zobacz [Omówienie narzędzia dostosowywania pakietu Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).

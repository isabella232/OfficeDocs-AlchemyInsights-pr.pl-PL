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
# <a name="using-the-office-deployment-tool-odt"></a>Przy użyciu narzędzia do wdrażania pakietu Office (ODT)

Narzędzie wdrażania pakietu Office (ODT) umożliwia wdrażanie wersji Office 365 pakietu Office. Narzędzia do wdrażania pakietu Office (setup.exe) jest uruchamiany z wiersza polecenia i używa pliku XML konfiguracji ustalenie, jakie ustawienia mają zastosowanie podczas wdrażania pakietu Office.
  
1. Pobierz najnowszą wersję narzędzia wdrażania pakietu Office z witryny [Microsoft — Centrum pobierania](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Użyj [Narzędzia dostosowywania pakietu Office (OCT)](https://config.office.com) , aby wybrać preferencji dotyczących wdrożenia i utworzyć plik konfiguracji XML. Wyeksportować plik konfiguracyjny i umieść go lokalnie na tym samym folderze, w którym znajduje się setup.exe.

    **Uwaga:** Instalacja pakietu Office, które często występują problemy ze względu na niepoprawnie skonfigurowany lub malformatted plików konfiguracyjnych. Aby uniknąć takich problemów, zaleca się użyć narzędzia dostosowywania pakietu Office do tworzenia pliku konfiguracji. Można także importować istniejące pliki konfiguracyjne do narzędzia dostosowywania pakietu Office.

3. Z wiersza polecenia Przełącz się do lokalizacji, gdzie znajduje się setup.exe i uruchom narzędzie wdrażania pakietu Office w trybie pobierania i określ plik konfiguracji, który został zapisany. W tym przykładzie plik konfiguracyjny o nazwie Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Uruchom Narzędzie wdrażania pakietu Office w trybie skonfigurować i określić plik konfiguracji.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Uwaga:** W tym kroku należy uruchomić z komputera klienckiego, na którym chcesz zainstalować pakiet Office i musi mieć uprawnienia administratora lokalnego na tym komputerze.

Aby dowiedzieć się więcej na temat używania narzędzia wdrażania pakietu Office Office 365 ProPlus scenariuszy wdrażania, zobacz [Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Aby uzyskać więcej informacji dotyczących sposobu używania narzędzia dostosowywania pakietu Office zobacz [Omówienie narzędzia dostosowywania pakietu Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).

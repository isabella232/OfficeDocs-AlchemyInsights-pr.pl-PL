---
title: Pytania dotyczące korzystania z narzędzia Office wdrażania pakietu (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959693"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pytania dotyczące korzystania z narzędzia Office wdrażania pakietu (ODT)

Pobierz Office wdrażania z [Centrum pobierania Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Po pobraniu pliku uruchom plik wykonywalny wyodrębniając samodzielnie, który zawiera plik wykonywalny narzędzia wdrażania programu Office (setup.exe) i przykładowy plik konfiguracji (configuration.xml).
  
 **Aby wykluczyć lub usunąć Aplikacje Microsoft 365 dla przedsiębiorstw z komputerów klienckich:**
  
Podczas instalowania Aplikacje Microsoft 365 dla przedsiębiorstw możesz wykluczyć określone produkty. W tym celu postępuj zgodnie z instrukcjami instalowania Office z plikiem ODT, ale uwzględnij element ExcludeApp w pliku konfiguracji. Na przykład ten plik konfiguracji instaluje wszystkie produkty Aplikacje Microsoft 365 dla przedsiębiorstw z wyjątkiem Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Omówienie narzędzia Office wdrażania](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  


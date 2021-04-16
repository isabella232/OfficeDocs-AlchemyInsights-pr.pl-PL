---
title: Pytania dotyczące używania Narzędzia wdrażania pakietu Office (ODT)
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
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790342"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pytania dotyczące używania Narzędzia wdrażania pakietu Office (ODT)

Pobierz Narzędzie wdrażania pakietu Office z [Centrum pobierania Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Po pobraniu pliku uruchom plik wykonywalny wyodrębniania samodzielnie, który zawiera plik wykonywalny Narzędzia wdrażania pakietu Office (setup.exe) i przykładowy plik konfiguracji (configuration.xml).
  
 **Aby wykluczyć lub usunąć aplikacje platformy Microsoft 365 dla przedsiębiorstw z komputerów klienckich:**
  
Podczas instalowania aplikacji platformy Microsoft 365 dla przedsiębiorstw możesz wykluczyć określone produkty. W tym celu wykonaj instrukcje dotyczące instalowania pakietu Office przy użyciu pliku ODT, ale uwzględnij element ExcludeApp w pliku konfiguracji. Na przykład ten plik konfiguracji instaluje wszystkie aplikacje platformy Microsoft 365 dla produktów dla przedsiębiorstw z wyjątkiem programu Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  


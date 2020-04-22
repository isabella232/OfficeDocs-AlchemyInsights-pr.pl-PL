---
title: Pytania dotyczące korzystania z narzędzia wdrażania pakietu Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698068"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pytania dotyczące korzystania z narzędzia wdrażania pakietu Office (ODT)

Pobierz narzędzie wdrażania pakietu Office z [Centrum pobierania Firmy Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po pobraniu pliku uruchom samodzielnie wyodrębniający plik wykonywalny, który zawiera plik wykonywalny Narzędzia wdrażania pakietu Office (setup.exe) i przykładowy plik konfiguracyjny (configuration.xml).
  
 **Aby wykluczyć lub usunąć aplikacje usługi Microsoft 365 dla produktów dla przedsiębiorstw z komputerów klienckich:**
  
Podczas instalowania aplikacji usługi Microsoft 365 dla przedsiębiorstw można wykluczyć określone produkty. Aby to zrobić, wykonaj kroki dotyczące instalowania pakietu Office z ODT, ale dołącz excludeApp element w pliku konfiguracji. Na przykład ten plik konfiguracyjny instaluje wszystkie aplikacje microsoftu 365 dla produktów dla przedsiębiorstw z wyjątkiem programu Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  


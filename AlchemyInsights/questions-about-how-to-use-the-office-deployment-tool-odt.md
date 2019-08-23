---
title: Pytania dotyczące sposobu używania narzędzia wdrażania pakietu Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553550"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pytania dotyczące sposobu używania narzędzia wdrażania pakietu Office (ODT)

Pobierz narzędzie wdrażania pakietu Office z witryny [Microsoft — Centrum pobierania](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po pobraniu pliku, uruchom samorozpakowujący się plik wykonywalny, który zawiera narzędzie wdrażania pakietu Office pliku wykonywalnego (setup.exe) i przykładowy plik konfiguracyjny (configuration.xml).
  
 **Aby wykluczyć lub usunięcia produktów Office 365 ProPlus z komputerów klienckich:**
  
Podczas instalowania pakietu Office 365 ProPlus, można wykluczyć określonych produktów. Aby to zrobić, wykonaj kroki wymagane do zainstalowania pakietu Office z ODT, ale zawierać ExcludeApp element w pliku konfiguracyjnym. Na przykład ten plik konfiguracyjny instaluje wszystkie produkty Office 365 ProPlus z wyjątkiem programu Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  


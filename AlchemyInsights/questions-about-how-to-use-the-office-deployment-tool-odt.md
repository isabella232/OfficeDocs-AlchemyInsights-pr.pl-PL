---
title: Pytania dotyczące sposobu korzystania z narzędzia wdrażania pakietu Office (ODT)
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553550"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pytania dotyczące sposobu korzystania z narzędzia wdrażania pakietu Office (ODT)

Pobierz narzędzie wdrażania pakietu Office z [Centrum pobierania firmy Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po pobraniu pliku Uruchom samowyodrębniający się plik wykonywalny, który zawiera narzędzie do wdrażania pakietu Office (Setup. exe) i przykładowy plik konfiguracyjny (Configuration. xml).
  
 **Aby wykluczyć lub usunąć produkty pakietu Office 365 ProPlus z komputerów klienckich:**
  
Podczas instalowania pakietu Office 365 ProPlus można wykluczyć określone produkty. Aby to zrobić, wykonaj kroki dotyczące instalowania pakietu Office z ODT, ale obejmują ExcludeApp element w pliku konfiguracyjnym. Na przykład ten plik konfiguracyjny instaluje wszystkie produkty pakietu Office 365 ProPlus z wyjątkiem programu Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  


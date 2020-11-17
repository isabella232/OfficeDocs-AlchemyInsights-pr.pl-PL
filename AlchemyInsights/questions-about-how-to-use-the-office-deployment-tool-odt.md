---
title: Pytania dotyczące korzystania z narzędzia wdrażania pakietu Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086166"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pytania dotyczące korzystania z narzędzia wdrażania pakietu Office (ODT)

Pobierz narzędzie wdrażania pakietu Office z [Centrum pobierania Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po pobraniu pliku Uruchom samowyodrębniający się plik wykonywalny, który zawiera plik wykonywalny narzędzia wdrażania pakietu Office (setupodt.exe) i przykładowy plik konfiguracji (configuration.xml).
  
 **Aby wykluczyć lub usunąć aplikacje Microsoft 365 dla produktów dla przedsiębiorstw z komputerów klienckich:**
  
Podczas instalowania aplikacji Microsoft 365 dla przedsiębiorstw możesz wykluczyć konkretne produkty. Aby to zrobić, postępuj zgodnie z instrukcjami instalowania pakietu Office za pomocą pliku ODT, ale Dołącz element ExcludeApp do pliku konfiguracji. Na przykład ten plik konfiguracyjny powoduje zainstalowanie wszystkich aplikacji Microsoft 365 dla przedsiębiorstw z wyjątkiem programu Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Omówienie narzędzia wdrażania pakietu Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  


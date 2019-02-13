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
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925354"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="112cc-102">Pytania dotyczące sposobu używania narzędzia wdrażania pakietu Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="112cc-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="112cc-103">Pobierz narzędzie wdrażania pakietu Office z witryny [Microsoft — Centrum pobierania](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="112cc-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="112cc-104">Po pobraniu pliku, uruchom samorozpakowujący się plik wykonywalny, który zawiera narzędzie wdrażania pakietu Office pliku wykonywalnego (setup.exe) i przykładowy plik konfiguracyjny (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="112cc-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="112cc-105">**Aby wykluczyć lub usunięcia produktów Office 365 ProPlus z komputerów klienckich:**</span><span class="sxs-lookup"><span data-stu-id="112cc-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="112cc-p101">Podczas instalowania pakietu Office 365 ProPlus, można wykluczyć określonych produktów. Aby to zrobić, wykonaj kroki wymagane do zainstalowania pakietu Office z ODT, ale zawierać ExcludeApp element w pliku konfiguracyjnym. Na przykład ten plik konfiguracyjny instaluje wszystkie produkty Office 365 ProPlus z wyjątkiem programu Publisher:</span><span class="sxs-lookup"><span data-stu-id="112cc-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="112cc-109">Omówienie narzędzia wdrażania pakietu Office</span><span class="sxs-lookup"><span data-stu-id="112cc-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  


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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="f7b4c-102">Pytania dotyczące sposobu używania narzędzia wdrażania pakietu Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="f7b4c-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="f7b4c-103">Pobierz narzędzie wdrażania pakietu Office z witryny [Microsoft — Centrum pobierania](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="f7b4c-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="f7b4c-104">Po pobraniu pliku, uruchom samorozpakowujący się plik wykonywalny, który zawiera narzędzie wdrażania pakietu Office pliku wykonywalnego (setup.exe) i przykładowy plik konfiguracyjny (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="f7b4c-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="f7b4c-105">**Aby wykluczyć lub usunięcia produktów Office 365 ProPlus z komputerów klienckich:**</span><span class="sxs-lookup"><span data-stu-id="f7b4c-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="f7b4c-106">Podczas instalowania pakietu Office 365 ProPlus, można wykluczyć określonych produktów.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="f7b4c-107">Aby to zrobić, wykonaj kroki wymagane do zainstalowania pakietu Office z ODT, ale zawierać ExcludeApp element w pliku konfiguracyjnym.</span><span class="sxs-lookup"><span data-stu-id="f7b4c-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="f7b4c-108">Na przykład ten plik konfiguracyjny instaluje wszystkie produkty Office 365 ProPlus z wyjątkiem programu Publisher:</span><span class="sxs-lookup"><span data-stu-id="f7b4c-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="f7b4c-109">Omówienie narzędzia wdrażania pakietu Office</span><span class="sxs-lookup"><span data-stu-id="f7b4c-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  


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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="d043d-102">Pytania dotyczące używania Narzędzia wdrażania pakietu Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="d043d-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="d043d-103">Pobierz Narzędzie wdrażania pakietu Office z [Centrum pobierania Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="d043d-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="d043d-104">Po pobraniu pliku uruchom plik wykonywalny wyodrębniania samodzielnie, który zawiera plik wykonywalny Narzędzia wdrażania pakietu Office (setup.exe) i przykładowy plik konfiguracji (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="d043d-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="d043d-105">**Aby wykluczyć lub usunąć aplikacje platformy Microsoft 365 dla przedsiębiorstw z komputerów klienckich:**</span><span class="sxs-lookup"><span data-stu-id="d043d-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="d043d-106">Podczas instalowania aplikacji platformy Microsoft 365 dla przedsiębiorstw możesz wykluczyć określone produkty.</span><span class="sxs-lookup"><span data-stu-id="d043d-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="d043d-107">W tym celu wykonaj instrukcje dotyczące instalowania pakietu Office przy użyciu pliku ODT, ale uwzględnij element ExcludeApp w pliku konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="d043d-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="d043d-108">Na przykład ten plik konfiguracji instaluje wszystkie aplikacje platformy Microsoft 365 dla produktów dla przedsiębiorstw z wyjątkiem programu Publisher:</span><span class="sxs-lookup"><span data-stu-id="d043d-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="d043d-109">Omówienie narzędzia wdrażania pakietu Office</span><span class="sxs-lookup"><span data-stu-id="d043d-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  


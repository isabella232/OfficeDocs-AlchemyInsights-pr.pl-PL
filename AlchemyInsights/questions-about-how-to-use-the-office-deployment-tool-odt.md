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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="c31d8-102">Pytania dotyczące korzystania z narzędzia wdrażania pakietu Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="c31d8-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="c31d8-103">Pobierz narzędzie wdrażania pakietu Office z [Centrum pobierania Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="c31d8-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="c31d8-104">Po pobraniu pliku Uruchom samowyodrębniający się plik wykonywalny, który zawiera plik wykonywalny narzędzia wdrażania pakietu Office (setupodt.exe) i przykładowy plik konfiguracji (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="c31d8-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="c31d8-105">**Aby wykluczyć lub usunąć aplikacje Microsoft 365 dla produktów dla przedsiębiorstw z komputerów klienckich:**</span><span class="sxs-lookup"><span data-stu-id="c31d8-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="c31d8-106">Podczas instalowania aplikacji Microsoft 365 dla przedsiębiorstw możesz wykluczyć konkretne produkty.</span><span class="sxs-lookup"><span data-stu-id="c31d8-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="c31d8-107">Aby to zrobić, postępuj zgodnie z instrukcjami instalowania pakietu Office za pomocą pliku ODT, ale Dołącz element ExcludeApp do pliku konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="c31d8-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="c31d8-108">Na przykład ten plik konfiguracyjny powoduje zainstalowanie wszystkich aplikacji Microsoft 365 dla przedsiębiorstw z wyjątkiem programu Publisher:</span><span class="sxs-lookup"><span data-stu-id="c31d8-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="c31d8-109">Omówienie narzędzia wdrażania pakietu Office</span><span class="sxs-lookup"><span data-stu-id="c31d8-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  


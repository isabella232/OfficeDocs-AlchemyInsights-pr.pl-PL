---
title: Zamień swoją klasyczną witrynę główną na nowoczesną witrynę
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741554"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="dffda-102">Zamień swoją klasyczną witrynę główną na nowoczesną witrynę</span><span class="sxs-lookup"><span data-stu-id="dffda-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="dffda-103">Jeśli środowisko zostało skonfigurowane przed kwietniem 2019 r., można zmienić witrynę główną na nowoczesną witrynę przy użyciu programu Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="dffda-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="dffda-104">Jeśli masz inną witrynę, której chcesz użyć jako witryny głównej, możesz zastąpić [ją (zamienić) witrynę główną.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="dffda-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="dffda-105">Użyj [invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) aby zamienić lokalizację lokacji z inną witryną podczas archiwizowania oryginalnej witryny.</span><span class="sxs-lookup"><span data-stu-id="dffda-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="dffda-106">Dostępne zarówno dla witryny zespołu (niepodłączonej do grupy), jak i dla witryny komunikacyjnej.</span><span class="sxs-lookup"><span data-stu-id="dffda-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="dffda-107">Wkrótce zostaną wprowadzone dodatkowe funkcje, które pozwolą ci nadal korzystać z zawartości witryny, ale przekonwertować istniejącą witrynę na witrynę komunikacyjną.</span><span class="sxs-lookup"><span data-stu-id="dffda-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="dffda-108">Możliwości te będą wprowadzane stopniowo.</span><span class="sxs-lookup"><span data-stu-id="dffda-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="dffda-109">Kontynuuj sprawdzanie aktualizacji w Centrum wiadomości.</span><span class="sxs-lookup"><span data-stu-id="dffda-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="dffda-110">Znane problemy z zamianą witryn</span><span class="sxs-lookup"><span data-stu-id="dffda-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="dffda-111">Witryna docelowa może zwrócić błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.</span><span class="sxs-lookup"><span data-stu-id="dffda-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="dffda-112">Zawartość będzie musiała zostać ponownie zindeksowana, aby zaktualizować indeks wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="dffda-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="dffda-113">Nie jest wymagany żaden ręczny krok - zostanie to zrobione automatycznie.</span><span class="sxs-lookup"><span data-stu-id="dffda-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="dffda-114">Wszystko, co zależy od "statycznych" łączy (takich jak synchronizacja plików i pliki programu OneNote) będzie musiało zostać ręcznie poprawione.</span><span class="sxs-lookup"><span data-stu-id="dffda-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="dffda-115">Jeśli witryna źródłowsza była witryną wiadomości organizacji, zaktualizuj adres URL.</span><span class="sxs-lookup"><span data-stu-id="dffda-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="dffda-116">Pobierz listę wszystkich witryn z wiadomościami organizacyjnymi.</span><span class="sxs-lookup"><span data-stu-id="dffda-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="dffda-117">Witryny programu Project Server mogą wymagać sprawdzenia poprawności, aby upewnić się, że są one nadal poprawnie skojarzone.</span><span class="sxs-lookup"><span data-stu-id="dffda-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>

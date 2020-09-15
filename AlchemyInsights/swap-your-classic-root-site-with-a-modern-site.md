---
title: Zamienianie klasycznej witryny głównej na witrynę Modern
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691189"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="851ea-102">Zamienianie klasycznej witryny głównej na witrynę Modern</span><span class="sxs-lookup"><span data-stu-id="851ea-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="851ea-103">Jeśli Twoje środowisko zostało skonfigurowane przed wydaniem 2019 kwietnia, możesz zmienić witrynę główną na witrynę Modern za pomocą programu Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="851ea-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="851ea-104">Jeśli masz inną witrynę, która ma być używana jako witryna główna, możesz zamienić ją [na witrynę główną (zamieniać](https://docs.microsoft.com/sharepoint/modern-root-site) się na nią).</span><span class="sxs-lookup"><span data-stu-id="851ea-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="851ea-105">Użyj funkcji [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , aby zamienić lokalizację witryny na inną witrynę podczas archiwizacji oryginalnej witryny.</span><span class="sxs-lookup"><span data-stu-id="851ea-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="851ea-106">Dostępne w przypadku witryny zespołu (niepołączonej z grupą) i witryny do komunikacji.</span><span class="sxs-lookup"><span data-stu-id="851ea-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="851ea-107">Zostaną wkrótce wprowadzone dodatkowe funkcje, które umożliwią korzystanie z zawartości witryny, ale Konwertowanie istniejącej witryny na witrynę komunikacyjną.</span><span class="sxs-lookup"><span data-stu-id="851ea-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="851ea-108">Te funkcje zostaną stopniowo rozwijane.</span><span class="sxs-lookup"><span data-stu-id="851ea-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="851ea-109">Kontynuuj sprawdzanie aktualizacji w centrum wiadomości.</span><span class="sxs-lookup"><span data-stu-id="851ea-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="851ea-110">Znane problemy dotyczące wymiany witryn</span><span class="sxs-lookup"><span data-stu-id="851ea-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="851ea-111">Witryna docelowa może zwracać błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.</span><span class="sxs-lookup"><span data-stu-id="851ea-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="851ea-112">Aby zaktualizować indeks wyszukiwania, zawartość musi zostać przeszukana ponownie.</span><span class="sxs-lookup"><span data-stu-id="851ea-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="851ea-113">Nie jest wymagany ręczny krok — zostanie on wykonany automatycznie.</span><span class="sxs-lookup"><span data-stu-id="851ea-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="851ea-114">Wszystkie osoby zależne od linków "static" (takie jak synchronizacja plików i pliki programu OneNote) trzeba będzie ręcznie poprawić.</span><span class="sxs-lookup"><span data-stu-id="851ea-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="851ea-115">Jeśli witryna źródłowa była witryną grup dyskusyjnych, zaktualizuj adres URL.</span><span class="sxs-lookup"><span data-stu-id="851ea-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="851ea-116">Zapoznaj się z listą wszystkich witryn z informacjami organizacyjnymi.</span><span class="sxs-lookup"><span data-stu-id="851ea-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="851ea-117">Witryny programu Project Server mogą wymagać sprawdzenia, aby upewnić się, że są nadal poprawnie skojarzone.</span><span class="sxs-lookup"><span data-stu-id="851ea-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>

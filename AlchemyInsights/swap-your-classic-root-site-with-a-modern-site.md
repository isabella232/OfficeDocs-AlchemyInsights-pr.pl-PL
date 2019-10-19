---
title: Zamień swoją stronę główną Classic z nowoczesnym miejscu
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749270"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="af02e-102">Zamień swoją stronę główną Classic z nowoczesnym miejscu</span><span class="sxs-lookup"><span data-stu-id="af02e-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="af02e-103">Jeśli środowisko zostało skonfigurowane przed kwietniem 2019, można zmienić witryny głównej do nowoczesnej witryny przy użyciu programu Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="af02e-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="af02e-104">Jeśli masz inną witrynę, która ma być używany jako witryny głównej, można zastąpić [(swap) witryny głównej](https://docs.microsoft.com/sharepoint/modern-root-site) z nim.</span><span class="sxs-lookup"><span data-stu-id="af02e-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="af02e-105">Użyj [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) do zamiany lokalizacji witryny z innej witryny podczas archiwizacji oryginalnej witryny.</span><span class="sxs-lookup"><span data-stu-id="af02e-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="af02e-106">Dostępne zarówno dla witryny zespołu (niepołączonej z grupą), jak i witryny komunikacyjnej.</span><span class="sxs-lookup"><span data-stu-id="af02e-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="af02e-107">Wkrótce zostaną wprowadzone dodatkowe możliwości, które pozwolą na dalsze korzystanie z zawartości witryny, ale przekonwertowanie istniejącej witryny na witrynę komunikacyjną.</span><span class="sxs-lookup"><span data-stu-id="af02e-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="af02e-108">Te możliwości będą wprowadzane stopniowo.</span><span class="sxs-lookup"><span data-stu-id="af02e-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="af02e-109">Kontynuuj sprawdzanie centrum wiadomości pakietu Office 365 dla aktualizacji.</span><span class="sxs-lookup"><span data-stu-id="af02e-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="af02e-110">Znane problemy z zamianę witryn</span><span class="sxs-lookup"><span data-stu-id="af02e-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="af02e-111">Witryna docelowa może zwracać błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.</span><span class="sxs-lookup"><span data-stu-id="af02e-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="af02e-112">Aby zaktualizować indeks wyszukiwania, konieczne będzie ponowne zaindeksowanie zawartości.</span><span class="sxs-lookup"><span data-stu-id="af02e-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="af02e-113">Nie jest wymagane ręczne krok-to będzie zrobione automatycznie.</span><span class="sxs-lookup"><span data-stu-id="af02e-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="af02e-114">Wszystko, co jest zależne od "statyczne" łącza (takie jak pliki synchronizacji plików i OneNote) należy ręcznie skorygować.</span><span class="sxs-lookup"><span data-stu-id="af02e-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="af02e-115">Jeśli witryna źródłowa była witryną wiadomości organizacji, zaktualizuj adres URL.</span><span class="sxs-lookup"><span data-stu-id="af02e-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="af02e-116">Uzyskaj listę wszystkich serwisów informacyjnych organizacji.</span><span class="sxs-lookup"><span data-stu-id="af02e-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="af02e-117">Witryny programu Project Server może wymagać sprawdzania poprawności, aby upewnić się, że są nadal skojarzone poprawnie.</span><span class="sxs-lookup"><span data-stu-id="af02e-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>






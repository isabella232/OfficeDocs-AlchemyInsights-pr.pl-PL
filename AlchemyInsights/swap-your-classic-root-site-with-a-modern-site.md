---
title: Zamień Classic głównej witrynie z nowoczesnymi witryny
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
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246041"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="6503b-102">Zamień Classic głównej witrynie z nowoczesnymi witryny</span><span class="sxs-lookup"><span data-stu-id="6503b-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="6503b-103">Jeśli środowisku była skonfigurowana przed 2019 kwietnia, można zmienić głównej witrynie do nowoczesnego witryny za pomocą Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="6503b-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="6503b-104">Jeśli masz inną witrynę, którą chcesz używać jako głównej witrynie można zastąpić (wymiany) katalogu głównego witryny z nim.</span><span class="sxs-lookup"><span data-stu-id="6503b-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="6503b-105">Użyj [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Aby zamienić lokalizację witryny z innej witryny podczas archiwizowania oryginalnej witryny.</span><span class="sxs-lookup"><span data-stu-id="6503b-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="6503b-106">Dostępne zarówno dla (nie połączeni z grupą) witryny zespołu i witryny komunikacji.</span><span class="sxs-lookup"><span data-stu-id="6503b-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="6503b-107">Dodatkowe możliwości pojawią się wkrótce pozwoli Ci utrzymać korzystania z zawartości w witrynie, ale Konwertowanie istniejącej witryny do witryny komunikacji.</span><span class="sxs-lookup"><span data-stu-id="6503b-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="6503b-108">Te możliwości będzie wdrażany stopniowo.</span><span class="sxs-lookup"><span data-stu-id="6503b-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="6503b-109">Nadal sprawdzać Centrum Office 365 wiadomości dla aktualizacji.</span><span class="sxs-lookup"><span data-stu-id="6503b-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="6503b-110">Znane problemy związane z zamiana stron</span><span class="sxs-lookup"><span data-stu-id="6503b-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="6503b-111">Witryna docelowa może zwrócić "nie znaleziono" błąd (HTTP 404) krótki okres czasu.</span><span class="sxs-lookup"><span data-stu-id="6503b-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="6503b-112">Zawartość będzie musiał być wykonane ponowne przeszukiwanie indeksu wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="6503b-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="6503b-113">Nie procesu ręcznego wymagane - ten odbywa się automatycznie.</span><span class="sxs-lookup"><span data-stu-id="6503b-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="6503b-114">Wszystko zależy od "static" łączy (na przykład pliki synchronizacji plików i program OneNote) będzie musiał ręcznie korygowana.</span><span class="sxs-lookup"><span data-stu-id="6503b-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="6503b-115">Jeśli źródłowa witryna witryny wiadomości dotyczące organizacji, należy zaktualizować adres URL.</span><span class="sxs-lookup"><span data-stu-id="6503b-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="6503b-116">Wyświetlić listę wszystkich witryn wiadomości dotyczące organizacji.</span><span class="sxs-lookup"><span data-stu-id="6503b-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="6503b-117">Project Server witryn może muszą zostać zatwierdzone do zapewnienia, że są nadal skojarzona poprawnie.</span><span class="sxs-lookup"><span data-stu-id="6503b-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>






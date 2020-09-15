---
title: Witryna Modern jako witryna główna
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666880"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="13c44-102">Witryna Modern jako witryna główna</span><span class="sxs-lookup"><span data-stu-id="13c44-102">Modern site as root site</span></span>

<span data-ttu-id="13c44-103">Rozpoczęto wprowadzanie nowej funkcji, która umożliwi [zamianę klasycznej witryny głównej witryny na witrynę Modern](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="13c44-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="13c44-104">Użyj funkcji [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , aby zamienić lokalizację witryny na inną witrynę podczas archiwizacji oryginalnej witryny.</span><span class="sxs-lookup"><span data-stu-id="13c44-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="13c44-105">Dostępne w przypadku witryny zespołu (niepołączonej z grupą) i witryny do komunikacji.</span><span class="sxs-lookup"><span data-stu-id="13c44-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="13c44-106">Nie usuwaj klasycznej witryny głównej, aby utworzyć nowoczesne witryny komunikacyjne.</span><span class="sxs-lookup"><span data-stu-id="13c44-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="13c44-107">Nie jest to obsługiwane przez firmę Microsoft.</span><span class="sxs-lookup"><span data-stu-id="13c44-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="13c44-108">Usunięcie witryny głównej spowoduje, że we wszystkich witrynach programu SharePoint w Twojej organizacji będzie ona niedostępna do wszystkich użytkowników, do momentu przywrócenia witryny lub utworzenia nowej witryny pod tym samym adresem URL.</span><span class="sxs-lookup"><span data-stu-id="13c44-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="13c44-109">Ta funkcja będzie przekazywana za pośrednictwem centrum wiadomości.</span><span class="sxs-lookup"><span data-stu-id="13c44-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="13c44-110">Należy się spodziewać, że ta funkcja została wkrótce włączona w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="13c44-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="13c44-111">Znane problemy dotyczące wymiany witryn</span><span class="sxs-lookup"><span data-stu-id="13c44-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="13c44-112">Witryna docelowa może zwracać błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.</span><span class="sxs-lookup"><span data-stu-id="13c44-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="13c44-113">Aby zaktualizować indeks wyszukiwania, zawartość musi zostać przeszukana ponownie.</span><span class="sxs-lookup"><span data-stu-id="13c44-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="13c44-114">W tym miejscu nie jest wymagane ręczne wykonanie tego kroku, zostanie ono automatycznie ukończone.</span><span class="sxs-lookup"><span data-stu-id="13c44-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="13c44-115">Wszystkie osoby zależne od linków "static" (takie jak synchronizacja plików i pliki programu OneNote) trzeba będzie ręcznie poprawić.</span><span class="sxs-lookup"><span data-stu-id="13c44-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="13c44-116">Witryny programu Project Server mogą wymagać sprawdzenia, aby upewnić się, że są nadal poprawnie skojarzone.</span><span class="sxs-lookup"><span data-stu-id="13c44-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 

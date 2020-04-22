---
title: Nowoczesna strona jako strona główna
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713801"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="c629c-102">Nowoczesna strona jako strona główna</span><span class="sxs-lookup"><span data-stu-id="c629c-102">Modern site as root site</span></span>

<span data-ttu-id="c629c-103">Zaczęliśmy wdrażać nową funkcję, która pozwoli Ci [zamienić klasyczną witrynę główną witryny na nowoczesną witrynę.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="c629c-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="c629c-104">Użyj [invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) aby zamienić lokalizację lokacji z inną witryną podczas archiwizowania oryginalnej witryny.</span><span class="sxs-lookup"><span data-stu-id="c629c-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="c629c-105">Dostępne zarówno dla witryny zespołu (niepodłączonej do grupy), jak i dla witryny komunikacyjnej.</span><span class="sxs-lookup"><span data-stu-id="c629c-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="c629c-106">Nie usuwaj klasycznej witryny głównej, aby utworzyć nowoczesną witrynę komunikacyjną.</span><span class="sxs-lookup"><span data-stu-id="c629c-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="c629c-107">Nie jest to obsługiwane przez firmę Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c629c-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="c629c-108">Usunięcie witryny głównej spowoduje, że wszystkie witryny programu SharePoint w organizacji staną się niedostępne dla wszystkich użytkowników, dopóki nie przywrócisz witryny lub nie utworzysz nowej witryny pod tym samym adresem URL.</span><span class="sxs-lookup"><span data-stu-id="c629c-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="c629c-109">Będziemy komunikować tę funkcję za pośrednictwem centrum wiadomości.</span><span class="sxs-lookup"><span data-stu-id="c629c-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="c629c-110">Należy się spodziewać, że funkcja zostanie wkrótce włączona w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="c629c-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="c629c-111">Znane problemy z zamianą witryn</span><span class="sxs-lookup"><span data-stu-id="c629c-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="c629c-112">Witryna docelowa może zwrócić błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.</span><span class="sxs-lookup"><span data-stu-id="c629c-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="c629c-113">Zawartość będzie musiała zostać ponownie zindeksowana, aby zaktualizować indeks wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="c629c-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="c629c-114">Nie jest tu wymagany żaden ręczny krok, zostanie to zrobione automatycznie.</span><span class="sxs-lookup"><span data-stu-id="c629c-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="c629c-115">Wszystko, co zależy od "statycznych" łączy (takich jak synchronizacja plików i pliki programu OneNote) będzie musiało zostać ręcznie poprawione.</span><span class="sxs-lookup"><span data-stu-id="c629c-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="c629c-116">Witryny programu Project Server mogą wymagać sprawdzenia poprawności, aby upewnić się, że są one nadal poprawnie skojarzone.</span><span class="sxs-lookup"><span data-stu-id="c629c-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 

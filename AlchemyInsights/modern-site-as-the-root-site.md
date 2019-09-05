---
title: Nowoczesna Strona jako Strona główna
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753914"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="493ec-102">Nowoczesna Strona jako Strona główna</span><span class="sxs-lookup"><span data-stu-id="493ec-102">Modern site as root site</span></span>

<span data-ttu-id="493ec-103">Zaczęliśmy wdrożyć nową funkcję, która pozwoli Ci [zamienić swoją klasyczną stronę główną witryny z nowoczesną stroną](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="493ec-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="493ec-104">Użyj [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) do zamiany lokalizacji witryny z innej witryny podczas archiwizacji oryginalnej witryny.</span><span class="sxs-lookup"><span data-stu-id="493ec-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="493ec-105">Dostępne zarówno dla witryny zespołu (niepołączonej z grupą), jak i witryny komunikacyjnej.</span><span class="sxs-lookup"><span data-stu-id="493ec-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="493ec-106">Nie usuwaj klasycznej witryny głównej, aby utworzyć nowoczesną witrynę komunikacyjną.</span><span class="sxs-lookup"><span data-stu-id="493ec-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="493ec-107">Nie jest to obsługiwane przez firmę Microsoft.</span><span class="sxs-lookup"><span data-stu-id="493ec-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="493ec-108">Usunięcie witryny głównej spowoduje, że wszystkie witryny programu SharePoint w organizacji będą niedostępne dla wszystkich użytkowników, dopóki nie przywrócisz witryny lub nie utworzysz nowej witryny pod tym samym adresem URL.</span><span class="sxs-lookup"><span data-stu-id="493ec-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="493ec-109">Będziemy komunikować tę funkcję za pośrednictwem centrum wiadomości.</span><span class="sxs-lookup"><span data-stu-id="493ec-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="493ec-110">Należy się spodziewać funkcji, które mają być włączone w dzierżawie wkrótce.</span><span class="sxs-lookup"><span data-stu-id="493ec-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="493ec-111">Znane problemy z zamianę witryn</span><span class="sxs-lookup"><span data-stu-id="493ec-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="493ec-112">Witryna docelowa może zwracać błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.</span><span class="sxs-lookup"><span data-stu-id="493ec-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="493ec-113">Aby zaktualizować indeks wyszukiwania, konieczne będzie ponowne zaindeksowanie zawartości.</span><span class="sxs-lookup"><span data-stu-id="493ec-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="493ec-114">Tu jest nie ręczny krok wymagany tutaj, ten mają być sporządzony mechanicznie.</span><span class="sxs-lookup"><span data-stu-id="493ec-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="493ec-115">Wszystko, co jest zależne od "statyczne" łącza (takie jak pliki synchronizacji plików i OneNote) należy ręcznie skorygować.</span><span class="sxs-lookup"><span data-stu-id="493ec-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="493ec-116">Witryny programu Project Server może wymagać sprawdzania poprawności, aby upewnić się, że są nadal skojarzone poprawnie.</span><span class="sxs-lookup"><span data-stu-id="493ec-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 

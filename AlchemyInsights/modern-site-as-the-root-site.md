---
title: Nowoczesne witryny jako witryny głównej
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
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543863"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="5cd28-102">Nowoczesne witryny jako witryny głównej</span><span class="sxs-lookup"><span data-stu-id="5cd28-102">Modern site as root site</span></span>

<span data-ttu-id="5cd28-103">Rozpoczęliśmy do rozmieszczenia nową funkcję, która pozwoli Ci o zamianę klasycznej strony głównej witrynie z nowoczesnymi witryny.</span><span class="sxs-lookup"><span data-stu-id="5cd28-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="5cd28-104">Użyj [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Aby zamienić lokalizację witryny z innej witryny podczas archiwizowania oryginalnej witryny.</span><span class="sxs-lookup"><span data-stu-id="5cd28-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="5cd28-105">Dostępne zarówno dla (nie połączeni z grupą) witryny zespołu i witryny komunikacji.</span><span class="sxs-lookup"><span data-stu-id="5cd28-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="5cd28-106">Nie należy usuwać klasyczny głównej witrynie do tworzenia nowoczesnych witryny komunikacji.</span><span class="sxs-lookup"><span data-stu-id="5cd28-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="5cd28-107">Nie jest to obsługiwane przez firmę Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cd28-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="5cd28-108">Usunięcie katalogu głównego witryny spowoduje, że wszystkie witryny programu SharePoint w organizacji niedostępne dla wszystkich użytkowników, dopóki Przywracanie witryny lub utworzyć nową witrynę o takim samym adresie URL.</span><span class="sxs-lookup"><span data-stu-id="5cd28-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="5cd28-109">Firma Microsoft będzie komunikować się tej funkcji za pośrednictwem Centrum wiadomości.</span><span class="sxs-lookup"><span data-stu-id="5cd28-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="5cd28-110">Należy się spodziewać funkcji należy włączyć w dzierżawie wkrótce.</span><span class="sxs-lookup"><span data-stu-id="5cd28-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="5cd28-111">Znane problemy związane z zamiana stron</span><span class="sxs-lookup"><span data-stu-id="5cd28-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="5cd28-112">Witryna docelowa może zwrócić "nie znaleziono" błąd (HTTP 404) krótki okres czasu.</span><span class="sxs-lookup"><span data-stu-id="5cd28-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="5cd28-113">Zawartość będzie musiał być wykonane ponowne przeszukiwanie indeksu wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="5cd28-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="5cd28-114">Nie procesu ręcznego tutaj, ten odbywa się automatycznie.</span><span class="sxs-lookup"><span data-stu-id="5cd28-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="5cd28-115">Wszystko zależy od "static" łączy (na przykład pliki synchronizacji plików i program OneNote) będzie musiał ręcznie korygowana.</span><span class="sxs-lookup"><span data-stu-id="5cd28-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="5cd28-116">Project Server witryn może muszą zostać zatwierdzone do zapewnienia, że są nadal skojarzona poprawnie.</span><span class="sxs-lookup"><span data-stu-id="5cd28-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 

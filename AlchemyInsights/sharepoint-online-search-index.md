---
title: Wyszukiwanie w usłudze SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f790efbe6ed445786933efa3fc980f974693d1d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770777"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="aa1a2-102">Przeszukiwanie zawartości i indeksowanie zawartości w usłudze SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="aa1a2-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="aa1a2-103">Zawartość musi zostać przeszukana i dodana do indeksu wyszukiwania dla użytkowników w celu znalezienia wyszukiwania w usłudze SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="aa1a2-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="aa1a2-104">Upewnij się, że zawartość witryny można znaleźć, [przedając jej możliwość wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="aa1a2-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="aa1a2-105">Po zmianie właściwości zarządzanej lub zmianie mapowania właściwości przeszukanych i zarządzanych należy ponownie przeszukać witrynę, zanim zmiany zostaną odzwierciedlone w indeksie wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="aa1a2-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="aa1a2-106">Aby uzyskać więcej informacji, zobacz [Ręczne żądanie przeszukiwania i ponowne indeksowanie witryny, biblioteki lub listy](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="aa1a2-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="aa1a2-107">Odczekaj co najmniej 24 godziny od ręcznego zażądania przeszukiwania i pełnego indeksu, aby sprawdzić, czy nadal występują problemy.</span><span class="sxs-lookup"><span data-stu-id="aa1a2-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="aa1a2-108">Jeśli od momentu zainicjowania przeszukiwania i pełnego indeksu upłynęło więcej niż 24 godziny, zarejestruj sprawę obsługi.</span><span class="sxs-lookup"><span data-stu-id="aa1a2-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="aa1a2-109">W wielu przypadkach jesteśmy już nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="aa1a2-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="aa1a2-110">Przekaż nam co najmniej 24 godziny na zakończenie rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="aa1a2-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="aa1a2-111">**Ważne**: Jeśli witryna, dokument (Biblioteka) lub lista została usunięta, a mimo to są wyświetlane w wynikach wyszukiwania, użytkownicy powinni otrzymać **błąd 404** podczas próby uzyskania dostępu do pliku.</span><span class="sxs-lookup"><span data-stu-id="aa1a2-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="aa1a2-112">Ten problem powinien być rejestrowany jako przypadek pomocy technicznej, aby uzyskać dalsze badania.</span><span class="sxs-lookup"><span data-stu-id="aa1a2-112">This issue should be logged as a support case for further investigation.</span></span>




---
title: Wyszukiwanie w programie SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044053"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="164c4-102">Indeksowanie zawartości i indeksowania w programie SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="164c4-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="164c4-103">Zawartość musi być przeszukiwany i dodawany do indeksu wyszukiwania dla użytkowników, aby znaleźć to, czego szukają w programie SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="164c4-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="164c4-104">Zawartość jest automatycznie przeszukiwany na podstawie wstępnie zdefiniowanego harmonogramu przeszukiwania (nie można zmienić harmonogramu przeszukiwania).</span><span class="sxs-lookup"><span data-stu-id="164c4-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="164c4-105">Przeszukiwarka przejmuje zawartość, która zmieniła się od czasu ostatniego przeszukiwania i aktualizuje indeks.</span><span class="sxs-lookup"><span data-stu-id="164c4-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="164c4-106">Aby upewnić się, że zawartość jest przeszukowana, a indeks jest aktualizowany, należy zwrócić uwagę na następujące elementy:</span><span class="sxs-lookup"><span data-stu-id="164c4-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="164c4-107">Upewnij się, że zawartość może zostać znaleziona poprzez [przeszukanie zawartości witryny](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="164c4-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="164c4-108">Po zmianie właściwości zarządzanej lub zmianie mapowania właściwości przeszukanych i zarządzanych lokacja musi zostać ponownie przeszukana, zanim zmiany zostaną odzwierciedlone w indeksie wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="164c4-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="164c4-109">Ponieważ zmiany są wprowadzane w schemacie wyszukiwania, a nie do rzeczywistej witryny, przeszukiwarka nie będzie automatycznie ponownie indeksować witryny.</span><span class="sxs-lookup"><span data-stu-id="164c4-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="164c4-110">Aby uzyskać więcej informacji, zobacz [Ręczne żądanie indeksowania i ponownego indeksowania witryny, biblioteki lub listy](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="164c4-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="164c4-111">Poczekaj co najmniej 24 godziny po ręcznym zażądaniu indeksowania i pełnego ponownego indeksowania, aby sprawdzić, czy nadal występuje problem.</span><span class="sxs-lookup"><span data-stu-id="164c4-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="164c4-112">Jeśli upłynęło więcej niż 24 godziny od zainicjowania indeksowania i pełnego ponownego indeksowania, należy zalogować się w przypadku pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="164c4-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="164c4-113">W wielu przypadkach pracujemy już nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="164c4-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="164c4-114">Proszę dać nam co najmniej 24 godziny, aby zakończyć rozwiązanie.</span><span class="sxs-lookup"><span data-stu-id="164c4-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="164c4-115">Jeśli witryna, dokument (Biblioteka) lub lista zostały usunięte i nadal są wyświetlane w wynikach wyszukiwania, użytkownicy powinni otrzymać **błąd 404 nie można odnaleźć pliku** podczas próby uzyskania do niego dostępu.</span><span class="sxs-lookup"><span data-stu-id="164c4-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="164c4-116">Ten problem powinien być rejestrowane jako przypadek pomocy technicznej do dalszego dochodzenia.</span><span class="sxs-lookup"><span data-stu-id="164c4-116">This issue should be logged as a support case for further investigation.</span></span> 




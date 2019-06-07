---
title: Zarządzanie słownikami Szukaj w dokumentacji Online programu SharePoint
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758775"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="9cc78-102">Wyszukaj w trybie Online w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="9cc78-102">Search in SharePoint Online</span></span>

<span data-ttu-id="9cc78-103">Zawartość musi przeszukanych i dodane do indeksu wyszukiwania użytkownikom znajdowanie, czego szukają w dokumentacji Online programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9cc78-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="9cc78-104">Automatycznie przeszukiwania zawartości oparty na harmonogram przeszukiwania wstępnie zdefiniowane (nie można zmienić harmonogram przeszukiwania).</span><span class="sxs-lookup"><span data-stu-id="9cc78-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="9cc78-105">Przeszukiwarka odbierze zawartość, która została zmieniona od czasu ostatniego przeszukiwania i aktualizuje indeks.</span><span class="sxs-lookup"><span data-stu-id="9cc78-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="9cc78-106">Aby zapewnić przeszukiwania zawartości i aktualizacji indeksu, wykonaj poniższe kroki.</span><span class="sxs-lookup"><span data-stu-id="9cc78-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="9cc78-107">Upewnij się, że zawartość znajduje się poprzez przeszukiwanie zawartości witryny.</span><span class="sxs-lookup"><span data-stu-id="9cc78-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="9cc78-108">Aby uzyskać więcej informacji zobacz [Włączanie treści na stronie ma być przeszukiwalna](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="9cc78-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="9cc78-109">Po zmianie właściwości zarządzanej lub po zmianie mapowanie przeszukany i zarządzane właściwości witryny musi być przeszukane ponownie, zanim wprowadzone zmiany zostaną odzwierciedlone w indeksie wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="9cc78-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="9cc78-110">Ponieważ Twoje zmiany zostaną wprowadzone w schematu wyszukiwania, a nie do rzeczywistej witryny przeszukiwarka nie zostaną automatycznie ponowne indeksowanie witryny.</span><span class="sxs-lookup"><span data-stu-id="9cc78-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="9cc78-111">Aby uzyskać więcej informacji zobacz temat [ręcznie zażądać i ponownego indeksowania danej witryny, listy lub biblioteki](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="9cc78-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="9cc78-112">Odczekaj co najmniej 24 godziny po zażądaniu ręcznie przeszukiwania i pełne ponowne indeksowanie aby zobaczyć, czy nadal występują problemu.</span><span class="sxs-lookup"><span data-stu-id="9cc78-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="9cc78-113">Jeśli więcej niż 24 godziny upłynęło od momentu zainicjowania przeszukiwania i pełne ponowne indeksowanie, należy zalogować się przypadek pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="9cc78-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="9cc78-114">W wielu przypadkach już pracujemy nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="9cc78-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9cc78-115">Podaj co najmniej 24 godziny, aby ukończyć rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="9cc78-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="9cc78-116">**Ważne**: Jeśli witryny, dokument (Biblioteka) lub listę usuniętych i nadal pokazuje w wynikach wyszukiwania, użytkownicy otrzymają błąd 404 Nie można odnaleźć pliku podczas próby uzyskania dostępu.</span><span class="sxs-lookup"><span data-stu-id="9cc78-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="9cc78-117">Ten problem powinny być rejestrowane jako przypadek pomocy technicznej w odniesieniu do dalszych badań.</span><span class="sxs-lookup"><span data-stu-id="9cc78-117">This issue should be logged as a support case for further investigation.</span></span> 




---
title: Zawartość nie jest widoczna w wynikach wyszukiwania programu SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363825"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="2a9bf-102">Zawartość nie jest widoczna w wynikach wyszukiwania programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="2a9bf-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="2a9bf-103">Wykonaj następujące kroki rozwiązywania problemów, gdy oczekiwana zawartość nie jest widoczna w wynikach wyszukiwania:</span><span class="sxs-lookup"><span data-stu-id="2a9bf-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="2a9bf-104">Sprawdź, czy **Witryna** zawiera oczekiwanej zawartości jest ustawione zezwalająca na zawartość pojawi się w wynikach wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="2a9bf-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="2a9bf-105">Postępuj zgodnie z instrukcjami [Pokaż zawartość witryny w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="2a9bf-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="2a9bf-106">Sprawdź **listę** lub **bibliotekę** , która zawiera oczekiwanej zawartości jest ustawiony zezwalająca na zawartość pojawi się w wynikach wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="2a9bf-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="2a9bf-107">Postępuj zgodnie z instrukcjami [Pokaż zawartość z listy lub biblioteki w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="2a9bf-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="2a9bf-108">Sprawdź, czy strony, dokumentu lub układ strony niestandardowe jest publikowany jako **wersja główna.**</span><span class="sxs-lookup"><span data-stu-id="2a9bf-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="2a9bf-109">Wykonaj krok 3 w [Wyszukiwanie nie zwraca wyników wszystkich w dokumentacji Online programu SharePoint](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="2a9bf-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="2a9bf-110">Sprawdź, czy użytkownik ma **uprawnienia** do wyświetlania zawartości.</span><span class="sxs-lookup"><span data-stu-id="2a9bf-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="2a9bf-111">Postępuj zgodnie z instrukcjami [zrozumienie poziomy uprawnień w programie SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="2a9bf-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="2a9bf-112">Jeśli zmieniono schematu wyszukiwania, dodając nową właściwość zarządzaną, edytując właściwości zarządzanej lub usuwając właściwości zarządzanej prośbą o przeszukiwanie i indeksowanie będzie wymagane.</span><span class="sxs-lookup"><span data-stu-id="2a9bf-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="2a9bf-113">**Ponowne indeksowanie** zawartości, wykonując kroki opisane w [ręcznie zażądać i ponownego indeksowania danej witryny, listy lub biblioteki](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="2a9bf-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="2a9bf-114">To może trochę potrwać, odczekać 24 godziny przed ponownym sprawdzaniem wyników.</span><span class="sxs-lookup"><span data-stu-id="2a9bf-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="2a9bf-115">Aby uzyskać więcej informacji zobacz [Włączanie treści na stronie ma być przeszukiwalna](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="2a9bf-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  

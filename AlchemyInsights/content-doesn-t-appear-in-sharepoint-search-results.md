---
title: Zawartość nie jest wyświetlana w wynikach wyszukiwania programu SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705671"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="aa1b7-102">Zawartość nie jest wyświetlana w wynikach wyszukiwania programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="aa1b7-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="aa1b7-103">Wykonaj następujące kroki rozwiązywania problemów, gdy oczekiwana zawartość nie jest wyświetlana w wynikach wyszukiwania:</span><span class="sxs-lookup"><span data-stu-id="aa1b7-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="aa1b7-104">Sprawdź, czy **witryna** zawierająca oczekiwaną zawartość jest ustawiona tak, aby zawartość wyświetlała się w wynikach wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="aa1b7-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="aa1b7-105">Wykonaj czynności opisane w obszarze [Pokazywalaj zawartość w witrynie w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="aa1b7-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="aa1b7-106">Sprawdź, czy **lista** lub **biblioteka zawierająca** oczekiwaną zawartość jest ustawiona tak, aby zawartość wyświetlała się w wynikach wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="aa1b7-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="aa1b7-107">Wykonaj czynności opisane w obszarze [Pokazywalaj zawartość z list lub bibliotek w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="aa1b7-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="aa1b7-108">Sprawdź, czy układ strony, dokumentu lub strony niestandardowej jest publikowany jako **wersja główna.**</span><span class="sxs-lookup"><span data-stu-id="aa1b7-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="aa1b7-109">Wykonaj krok 3 w [wyszukiwarce nie zwraca wszystkich wyników w usłudze SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="aa1b7-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="aa1b7-110">Sprawdź, czy użytkownik ma **uprawnienia** do wyświetlania zawartości.</span><span class="sxs-lookup"><span data-stu-id="aa1b7-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="aa1b7-111">Wykonaj kroki opisane w [opisie poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="aa1b7-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="aa1b7-112">Jeśli schemat wyszukiwania został zmieniony przez dodanie nowej właściwości zarządzanej, przez edycję właściwości zarządzanej lub przez usunięcie właściwości zarządzanej, wymagane będzie żądanie indeksowania i ponownego indeksowania.</span><span class="sxs-lookup"><span data-stu-id="aa1b7-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="aa1b7-113">**Ponownie indeksuj** zawartość, wykonując czynności opisane w [Ręcznym żądaniu indeksowania i ponownego indeksowania witryny, biblioteki lub listy](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="aa1b7-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="aa1b7-114">Może to trochę potrwać, odczekaj 24 godziny przed ponownym sprawdzeniem wyników.</span><span class="sxs-lookup"><span data-stu-id="aa1b7-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="aa1b7-115">Aby uzyskać więcej informacji, zobacz [Włączanie przeszukiwania zawartości witryny](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="aa1b7-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  

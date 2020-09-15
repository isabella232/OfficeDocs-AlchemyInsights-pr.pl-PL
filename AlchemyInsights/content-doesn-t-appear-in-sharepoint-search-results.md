---
title: Zawartość nie jest wyświetlana w wynikach wyszukiwania w programie SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713140"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="16a69-102">Zawartość nie jest wyświetlana w wynikach wyszukiwania w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="16a69-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="16a69-103">Wykonaj te czynności rozwiązywania problemów, gdy oczekiwana zawartość nie zostanie wyświetlona w wynikach wyszukiwania:</span><span class="sxs-lookup"><span data-stu-id="16a69-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="16a69-104">Sprawdź, czy **Witryna** zawierająca oczekiwaną zawartość jest ustawiona tak, aby zezwalać na wyświetlanie zawartości w wynikach wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="16a69-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="16a69-105">Wykonaj czynności podane w artykule [Pokazywanie zawartości witryny w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="16a69-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="16a69-106">Sprawdź, czy **Lista** lub **Biblioteka** zawierająca oczekiwaną zawartość jest ustawiona tak, aby zezwalać na wyświetlanie zawartości w wynikach wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="16a69-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="16a69-107">Postępuj zgodnie z instrukcjami podanymi w [artykule pokazywanie zawartości z list lub bibliotek w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="16a69-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="16a69-108">Sprawdź, czy strona, dokument lub niestandardowy układ strony jest opublikowany jako **wersja główna.**</span><span class="sxs-lookup"><span data-stu-id="16a69-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="16a69-109">Obserwuj krok 3 w funkcji [wyszukiwania nie są zwracane wszystkie wyniki w usłudze SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="16a69-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="16a69-110">Sprawdź, czy użytkownik ma **uprawnienia** do wyświetlania zawartości.</span><span class="sxs-lookup"><span data-stu-id="16a69-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="16a69-111">Postępuj zgodnie z instrukcjami podanymi w artykule [Omówienie poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="16a69-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="16a69-112">Jeśli schemat wyszukiwania został zmieniony przez dodanie nowej właściwości zarządzanej, edytując właściwość zarządzaną lub usuwając właściwość zarządzaną, wymagane jest ponowne przeszukiwanie i ponowne indeksowanie.</span><span class="sxs-lookup"><span data-stu-id="16a69-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="16a69-113">**Ponownie Indeksuj** zawartość, wykonując czynności opisane w temacie [Ręczne żądanie przeszukiwania i ponowne indeksowanie witryny, biblioteki lub listy](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="16a69-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="16a69-114">Może to trochę potrwać, odczekaj 24 godziny, zanim ponownie sprawdzisz wyniki.</span><span class="sxs-lookup"><span data-stu-id="16a69-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="16a69-115">Aby uzyskać więcej informacji, zobacz [Włączanie funkcji wyszukiwania zawartości w witrynie](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="16a69-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  

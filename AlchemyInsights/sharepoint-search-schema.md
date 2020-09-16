---
title: Zarządzanie schematem wyszukiwania w usłudze SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770561"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="6f242-102">Zarządzanie schematem wyszukiwania w usłudze SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6f242-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="6f242-103">Schemat wyszukiwania kontroluje, co użytkownicy mogą wyszukać, jak użytkownicy mogą je przeszukiwać, a także jak przedstawić wyniki w witrynach internetowych wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="6f242-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="6f242-104">Zobacz [Zarządzanie schematem wyszukiwania w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) , aby dowiedzieć się, jak to zrobić:</span><span class="sxs-lookup"><span data-stu-id="6f242-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="6f242-105">Zmienianie schematu wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="6f242-105">Change the search schema.</span></span>
- <span data-ttu-id="6f242-106">Tworzenie właściwości zarządzanych.</span><span class="sxs-lookup"><span data-stu-id="6f242-106">Create managed properties.</span></span>
- <span data-ttu-id="6f242-107">Mapowanie właściwości przeszukanych mapy przeszukanej na właściwości zarządzane.</span><span class="sxs-lookup"><span data-stu-id="6f242-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="6f242-108">Zwróć uwagę na następujące kwestie dotyczące zarządzania schematem wyszukiwania:</span><span class="sxs-lookup"><span data-stu-id="6f242-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="6f242-109">Jeśli zostanie wyświetlone ostrzeżenie informujące o tym, **że aplikacja została wstrzymana** w przypadku zmiany schematu, ta funkcja jest dostępna tylko tymczasowo, ponieważ ma miejsce konserwacja usługi.</span><span class="sxs-lookup"><span data-stu-id="6f242-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="6f242-110">Jeśli przekazano więcej niż 24 godziny i nadal występują ostrzeżenia, zarejestruj sprawę obsługi.</span><span class="sxs-lookup"><span data-stu-id="6f242-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="6f242-111">Po zmianie właściwości zarządzanych lub dodaniu nowych zmian zmiany zostaną wprowadzone dopiero po ponownym przeszukaniu zawartości.</span><span class="sxs-lookup"><span data-stu-id="6f242-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="6f242-112">W usłudze SharePoint Online przeszukiwanie jest wykonywane automatycznie na podstawie zdefiniowanego harmonogramu przeszukiwania.</span><span class="sxs-lookup"><span data-stu-id="6f242-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="6f242-113">Aby upewnić się, że zmiany są przeszukiwane, możesz szczególnie [zażądać ponownego indeksowania listy lub biblioteki](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="6f242-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="6f242-114">Aby zapoznać się z pełnym omówieniem schematu wyszukiwania, zobacz [wprowadzenie schematu wyszukiwania](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="6f242-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 



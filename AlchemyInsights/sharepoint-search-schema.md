---
title: Zarządzanie schematem wyszukiwania w programie SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042973"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="c1c19-102">Zarządzanie schematem wyszukiwania w programie SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c1c19-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="c1c19-103">Schemat wyszukiwania kontroluje, co użytkownicy mogą wyszukiwać, jak użytkownicy mogą wyszukiwać i jak można przedstawić wyniki w witrynach sieci Web wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="c1c19-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="c1c19-104">Zobacz [Zarządzanie schematem wyszukiwania w usłudze SharePoint Online,](https://docs.microsoft.com/sharepoint/manage-search-schema) aby dowiedzieć się, jak:</span><span class="sxs-lookup"><span data-stu-id="c1c19-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="c1c19-105">Zmień schemat wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="c1c19-105">Change the search schema.</span></span>
- <span data-ttu-id="c1c19-106">Tworzenie właściwości zarządzanych.</span><span class="sxs-lookup"><span data-stu-id="c1c19-106">Create managed properties.</span></span>
- <span data-ttu-id="c1c19-107">Mapy przeszukane mapy przeszukane właściwości do właściwości zarządzanych.</span><span class="sxs-lookup"><span data-stu-id="c1c19-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="c1c19-108">W odniesieniu do zarządzania schematem wyszukiwania należy zwrócić uwagę na następujące:</span><span class="sxs-lookup"><span data-stu-id="c1c19-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="c1c19-109">Jeśli zostanie wyświetlone ostrzeżenie z informacją, **że aplikacja jest wstrzymana** podczas wprowadzania zmian schematu, jest to tylko tymczasowe, ponieważ występuje konserwacja usługi.</span><span class="sxs-lookup"><span data-stu-id="c1c19-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="c1c19-110">Jeśli minęło więcej niż 24 godziny i nadal występują ostrzeżenia, należy zalogować się w przypadku pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="c1c19-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="c1c19-111">Po zmianie właściwości zarządzanych lub dodaniu nowych zmiany zostaną uwzględnione dopiero po ponownym przeszuknie zawartości.</span><span class="sxs-lookup"><span data-stu-id="c1c19-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="c1c19-112">W programie SharePoint Online indeksowanie odbywa się automatycznie na podstawie zdefiniowanego harmonogramu przeszukiwania.</span><span class="sxs-lookup"><span data-stu-id="c1c19-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="c1c19-113">Aby upewnić się, że zmiany są przeszukane, można w szczególności [zażądać ponownego indeksowania listy lub biblioteki](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="c1c19-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="c1c19-114">Aby uzyskać pełny przegląd schematu wyszukiwania, zobacz Wprowadzenie do [schematu wyszukiwania](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="c1c19-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 



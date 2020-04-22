---
title: 1491-search-not-returning-expected-results 1491-search-not-returning-expected-results 1491-search-not-returning-expected-results 1
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709237"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="c68ad-102">Wyszukiwanie zawartości nie zwraca oczekiwanych wyników</span><span class="sxs-lookup"><span data-stu-id="c68ad-102">Content Search not returning expected results</span></span>

<span data-ttu-id="c68ad-103">Podczas uruchamiania wyszukiwania zawartości z Centrum zgodności & zabezpieczeń usługi Microsoft 365 mogą pojawić się nieoczekiwane wyniki wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="c68ad-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="c68ad-104">Należy wziąć pod uwagę następujące kwestie, które mogą mieć wpływ na wyniki wyszukiwania:</span><span class="sxs-lookup"><span data-stu-id="c68ad-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="c68ad-105">**Lokalizacje zawartości i warunki wyszukiwania:** upewnij się, że wybrano odpowiednie lokalizacje zawartości i warunki wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="c68ad-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="c68ad-106">Jeśli uruchomiono duże wyszukiwanie (z wieloma lokalizacjami), rozważ podzielenie go na wiele wyszukiwań.</span><span class="sxs-lookup"><span data-stu-id="c68ad-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="c68ad-107">**Elementy częściowo indeksowane**: [Elementy częściowo indeksowane](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) ze skrzynek pocztowych są uwzględniane w szacowanych wynikach wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="c68ad-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="c68ad-108">Jednak elementy częściowo indeksowane z witryn w programie SharePoint i OneDrive nie są uwzględniane w szacowaniu wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="c68ad-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="c68ad-109">**Błędy wyszukiwania:** Podczas przeszukiwania dużej liczby skrzynek pocztowych (ponad 100 000 skrzynek pocztowych) mogą pojawić się błędy wyszukiwania, z kodami błędów, takimi jak CS008-009 i CS012-002).</span><span class="sxs-lookup"><span data-stu-id="c68ad-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="c68ad-110">W takim przypadku ponów próbę wyszukiwania tylko dla lokalizacji zawartości, które nie powiodło się.</span><span class="sxs-lookup"><span data-stu-id="c68ad-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="c68ad-111">Zobacz [ten artykuł,](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="c68ad-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>

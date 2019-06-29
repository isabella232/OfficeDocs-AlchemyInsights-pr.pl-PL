---
title: 1491-Search-not-Returning-expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355887"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="f94c9-102">Przeszukiwanie zawartości nie zwraca wyników oczekiwanych</span><span class="sxs-lookup"><span data-stu-id="f94c9-102">Content Search not returning expected results</span></span>

<span data-ttu-id="f94c9-103">Podczas uruchamiania wyszukiwania zawartości z & zabezpieczeń usługi Office 365 Centrum zgodności, może pojawić się nieoczekiwanych wyników.</span><span class="sxs-lookup"><span data-stu-id="f94c9-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="f94c9-104">Należy wziąć pod uwagę następujące rzeczy, które mogą wpływać na wyniki wyszukiwania:</span><span class="sxs-lookup"><span data-stu-id="f94c9-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="f94c9-105">**Lokalizacje zawartości i warunki wyszukiwania**: Upewnij się, wybraniu odpowiedniej lokalizacji zawartości i warunki wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="f94c9-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="f94c9-106">Jeśli uruchomiono dużych wyszukiwania (z wielu lokalizacji), należy rozważyć rozdzielenie go na wielu wyszukiwań.</span><span class="sxs-lookup"><span data-stu-id="f94c9-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="f94c9-107">**Częściowo indeksowanych elementów**: [częściowo indeksowanych elementów](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) ze skrzynek pocztowych są uwzględniane w wynikach wyszukiwania szacowany.</span><span class="sxs-lookup"><span data-stu-id="f94c9-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="f94c9-108">Jednak częściowo indeksowane elementy z witryn programu SharePoint i OneDrive nie są uwzględniane podczas szacowania wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="f94c9-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="f94c9-109">**Wyszukiwanie błędów**: podczas wyszukiwania dużą liczbę skrzynek pocztowych (ponad 100 000 skrzynek pocztowych), mogą wystąpić błędy wyszukiwania, z kodami błędów, takich jak CS008-009 i CS012-002).</span><span class="sxs-lookup"><span data-stu-id="f94c9-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="f94c9-110">W takim przypadku ponów próbę wyszukiwania tylko dla lokalizacji zawartości nie powiodło się.</span><span class="sxs-lookup"><span data-stu-id="f94c9-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="f94c9-111">Zobacz [Ten artykuł](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="f94c9-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>

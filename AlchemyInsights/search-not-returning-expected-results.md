---
title: 1491 — wyniki wyszukiwania, nieoczekiwane
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740484"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="f8321-102">Funkcja wyszukiwania zawartości nie zwraca oczekiwanych wyników</span><span class="sxs-lookup"><span data-stu-id="f8321-102">Content Search not returning expected results</span></span>

<span data-ttu-id="f8321-103">Podczas uruchamiania wyszukiwania zawartości z poziomu Centrum zgodności z & zabezpieczeniami programu Microsoft 365 mogą być wyświetlane nieoczekiwane wyniki wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="f8321-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="f8321-104">Uwzględnij następujące kwestie, które mogą mieć wpływ na wyniki wyszukiwania:</span><span class="sxs-lookup"><span data-stu-id="f8321-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="f8321-105">**Lokalizacje zawartości i warunki wyszukiwania**: Upewnij się, że wybrano odpowiednie lokalizacje zawartości i warunki wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="f8321-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="f8321-106">Jeśli uruchomiono duże wyszukiwanie (z wieloma lokalizacjami), warto je podzielić na wiele wyszukiwań.</span><span class="sxs-lookup"><span data-stu-id="f8321-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="f8321-107">**Częściowo indeksowane elementy**:  [częściowo indeksowane elementy](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) z skrzynek pocztowych są uwzględniane w szacowanych wynikach wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="f8321-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="f8321-108">Jednak częściowo indeksowane elementy z witryn w programie SharePoint i w usłudze OneDrive nie są uwzględniane w szacowaniu wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="f8321-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="f8321-109">**Błędy wyszukiwania**: podczas wyszukiwania dużej liczby skrzynek pocztowych (ponad 100 000 skrzynek pocztowych) możesz otrzymywać błędy wyszukiwania, korzystając z kodów błędów, takich jak CS008-009 i CS012-002).</span><span class="sxs-lookup"><span data-stu-id="f8321-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="f8321-110">W takim przypadku ponów wyszukiwanie tylko w przypadku niepowodzenia lokalizacji zawartości.</span><span class="sxs-lookup"><span data-stu-id="f8321-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="f8321-111">Aby uzyskać więcej informacji, zobacz  [ten artykuł](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="f8321-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

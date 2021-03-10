---
title: Stosowanie najlepszych rozwiązań dla zaawansowanych zapytań łowiecki
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696088"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="5d707-102">Stosowanie najlepszych rozwiązań dla zaawansowanych zapytań łowiecki</span><span class="sxs-lookup"><span data-stu-id="5d707-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="5d707-103">Aby szybciej uzyskać wyniki i uniknąć limitów czasu podczas uruchamiania złożonych zapytań, zastosuj poniższe najlepsze rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="5d707-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="5d707-104">Podczas próby nowych zapytań zawsze używaj limitu, aby uniknąć bardzo dużych zestawów wyników.</span><span class="sxs-lookup"><span data-stu-id="5d707-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="5d707-105">Ponadto skorzystaj `count` z tej funkcji, aby dokonać wstępnej oceny rozmiaru zestawu wyników.</span><span class="sxs-lookup"><span data-stu-id="5d707-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="5d707-106">Najpierw użyj filtrów czasu.</span><span class="sxs-lookup"><span data-stu-id="5d707-106">Use time filters first.</span></span> <span data-ttu-id="5d707-107">Najlepiej jest ograniczyć kwerendy do siedmiu dni.</span><span class="sxs-lookup"><span data-stu-id="5d707-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="5d707-108">Na początku zapytania, zaraz po filtrze czasu, dodaj filtry, które mają usunąć większość danych.</span><span class="sxs-lookup"><span data-stu-id="5d707-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="5d707-109">Gdy szukasz pełnych tokenów, użyj `has` operatora, a nie `contains` .</span><span class="sxs-lookup"><span data-stu-id="5d707-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="5d707-110">Uruchom wyszukiwanie dla określonej kolumny, a nie we wszystkich kolumnach.</span><span class="sxs-lookup"><span data-stu-id="5d707-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="5d707-111">Podczas dołączania do tabel najpierw określ tabelę z mniejszą liczbą wierszy.</span><span class="sxs-lookup"><span data-stu-id="5d707-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="5d707-112">`project` tylko niezbędne kolumny z tabel, które zostały sprzężenia.</span><span class="sxs-lookup"><span data-stu-id="5d707-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="5d707-113">Aby dowiedzieć się więcej, zobacz najlepsze rozwiązania [dotyczące zapytań wyszukiwania zaawansowanego.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="5d707-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>

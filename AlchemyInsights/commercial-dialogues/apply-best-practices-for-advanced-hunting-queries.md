---
title: Stosowanie najlepszych rozwiązań dla zaawansowanych zapytań myśliwnych
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749544"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="f81c7-102">Stosowanie najlepszych rozwiązań dla zaawansowanych zapytań myśliwnych</span><span class="sxs-lookup"><span data-stu-id="f81c7-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="f81c7-103">Aby szybciej uzyskać wyniki i uniknąć limitów czasu podczas uruchamiania złożonych zapytań, zastosuj następujące najlepsze rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="f81c7-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="f81c7-104">Podczas próby nowych zapytań zawsze używaj limitu, aby uniknąć uzyskiwania bardzo dużych zestawów wyników.</span><span class="sxs-lookup"><span data-stu-id="f81c7-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="f81c7-105">Ponadto skorzystaj z tej funkcji, aby dokonać wstępnej `count` oceny rozmiaru zestawu wyników.</span><span class="sxs-lookup"><span data-stu-id="f81c7-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="f81c7-106">Najpierw użyj filtrów czasu.</span><span class="sxs-lookup"><span data-stu-id="f81c7-106">Use time filters first.</span></span> <span data-ttu-id="f81c7-107">Najlepiej jest ograniczyć kwerendy do siedmiu dni.</span><span class="sxs-lookup"><span data-stu-id="f81c7-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="f81c7-108">Na początku zapytania, zaraz po filtrze czasu, dodaj filtry oczekiwane do usunięcia większości danych.</span><span class="sxs-lookup"><span data-stu-id="f81c7-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="f81c7-109">Gdy szukasz pełnych tokenów, `has` użyj operatora, a nie `contains` .</span><span class="sxs-lookup"><span data-stu-id="f81c7-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="f81c7-110">Wyszukiwanie należy uruchomić dla określonej kolumny, a nie we wszystkich kolumnach.</span><span class="sxs-lookup"><span data-stu-id="f81c7-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="f81c7-111">Podczas łączenia tabel najpierw określ tabelę z mniejszą liczbą wierszy.</span><span class="sxs-lookup"><span data-stu-id="f81c7-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="f81c7-112">`project` tylko niezbędne kolumny z tabel, do których zostały sprzężenia.</span><span class="sxs-lookup"><span data-stu-id="f81c7-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="f81c7-113">Aby dowiedzieć się więcej, zobacz Najlepsze rozwiązania [dla zapytania wyszukiwania zaawansowanego.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="f81c7-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>

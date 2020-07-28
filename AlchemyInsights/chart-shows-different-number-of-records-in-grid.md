---
title: Wykres pokazuje różną liczbę rekordów w siatce
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439967"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="cb33d-102">Wykres pokazuje różną liczbę rekordów w siatce</span><span class="sxs-lookup"><span data-stu-id="cb33d-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="cb33d-103">**Objawem**</span><span class="sxs-lookup"><span data-stu-id="cb33d-103">**Symptom**</span></span>

<span data-ttu-id="cb33d-104">W przypadku wykresu na stronie pulpitu nawigacyjnego po kliknięciu wykresu "..." i kliknij "Wyświetl rekordy", przejdź do strony siatki, aby wyświetlić wszystkie rekordy. Czasami zmienia się liczba rekordów.</span><span class="sxs-lookup"><span data-stu-id="cb33d-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="cb33d-105">**Przyczyna**</span><span class="sxs-lookup"><span data-stu-id="cb33d-105">**Cause**</span></span>

<span data-ttu-id="cb33d-106">Wynika to z różnicy widoków między wykresem na oryginalnej stronie pulpitu nawigacyjnego a wykresem na stronie głównej siatki.</span><span class="sxs-lookup"><span data-stu-id="cb33d-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="cb33d-107">**Rozwiązanie**</span><span class="sxs-lookup"><span data-stu-id="cb33d-107">**Solution**</span></span>

1. <span data-ttu-id="cb33d-108">Sprawdź widok z oryginalnej strony i widoku w siatce, aby sprawdzić, czy są różne.</span><span class="sxs-lookup"><span data-stu-id="cb33d-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="cb33d-109">Zmień widok w siatce, aby dopasować go do widoku na oryginalnej stronie.</span><span class="sxs-lookup"><span data-stu-id="cb33d-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="cb33d-110">Jeśli nie można znaleźć poprawnego widoku, zwykle oznacza to, że widok nie jest włączony w projektancie aplikacji.</span><span class="sxs-lookup"><span data-stu-id="cb33d-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="cb33d-111">Przejdź do projektanta aplikacji określonej aplikacji, wybierz encję i jej widoki, sprawdź widok, który chcesz włączyć, zapisać, opublikować i zamknąć.</span><span class="sxs-lookup"><span data-stu-id="cb33d-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="cb33d-112">Odśwież stronę.</span><span class="sxs-lookup"><span data-stu-id="cb33d-112">Refresh the page.</span></span>
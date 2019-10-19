---
title: tak samo jak nazwa pliku jest Najlepsza
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "35800055"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="97927-102">Wymagane Alchemy header H1, H2 nie działają.</span><span class="sxs-lookup"><span data-stu-id="97927-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="97927-103">Sprawdzone metody i wskazówki dotyczące tworzenia treści Alchemy:</span><span class="sxs-lookup"><span data-stu-id="97927-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="97927-104">**Nie zagnieżdżać Alchemy Insights w folderach**-spowoduje to przerwanie struktury URL.</span><span class="sxs-lookup"><span data-stu-id="97927-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="97927-105">Patrzymy na naprawienie tego.</span><span class="sxs-lookup"><span data-stu-id="97927-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="97927-106">Pliki w folderze **Alchemyinsights** powinny mieć małe nazwy plików z myślkami dla spacji ex.</span><span class="sxs-lookup"><span data-stu-id="97927-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="97927-107">***jak-wobec-umożliwiać-sądowym-Hold***.</span><span class="sxs-lookup"><span data-stu-id="97927-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="97927-108">Dołącz Identyfikator reguły lub identyfikator zasobnika z [portalu partnera Alchemy](https://alchemyportal.azurewebsites.net) w polu MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="97927-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="97927-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="97927-109">ex.</span></span> <span data-ttu-id="97927-110">***MS. zwyczaj: 100021***</span><span class="sxs-lookup"><span data-stu-id="97927-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="97927-111">Użyj pozostałej części metadanych w górnej części tego pliku jako szablonu.</span><span class="sxs-lookup"><span data-stu-id="97927-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="97927-112">W [portalu dla partnerów Alchemy](https://alchemyportal.azurewebsites.net)przejdź w dół do sekcji **Customer Insight title:** i wykorzystaj to jako punkt wyjścia dla swojego tytułu H1 dla wglądu.</span><span class="sxs-lookup"><span data-stu-id="97927-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="97927-113">Alchemy Insights musi mieć tylko jeden H1 na górze lub będą one złamać w produkcji.</span><span class="sxs-lookup"><span data-stu-id="97927-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="97927-114">H2s nie renderuje tak więc Użyj **pogrubienie** lub inne konwencje oznaczają oddzielne sekcje.</span><span class="sxs-lookup"><span data-stu-id="97927-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="97927-115">Następnie wypełnij tekst treści za pomocą materiałów roboczych w sekcji Customer Insights na stronie reguła alchemii.</span><span class="sxs-lookup"><span data-stu-id="97927-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="97927-116">Listy wypunktowane są w porządku</span><span class="sxs-lookup"><span data-stu-id="97927-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="97927-117">Listy numerowane zbyt</span><span class="sxs-lookup"><span data-stu-id="97927-117">Numbered lists too</span></span>
    1. <span data-ttu-id="97927-118">**Pogrubienie** i *kursywa* są-OK</span><span class="sxs-lookup"><span data-stu-id="97927-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="97927-119">Łącza zawsze powinny być albo **"łącza do sieci Web"/External** lub **Deep-łącza do elementów interfejsu użytkownika**, a nie wewnętrzne łącza.</span><span class="sxs-lookup"><span data-stu-id="97927-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="97927-120">Zdjęcia nie są oficjalnie wspierane w tej chwili, ale to na planie.</span><span class="sxs-lookup"><span data-stu-id="97927-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="97927-121">I to jest naprawdę już trochę za długo.</span><span class="sxs-lookup"><span data-stu-id="97927-121">And this is really already a bit too long.</span></span> <span data-ttu-id="97927-122">Najlepsze praktyki jest około 400 znaków---------------------------------</span><span class="sxs-lookup"><span data-stu-id="97927-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="97927-123">Gdy zawartość będzie gotowa, pociągnij ją do gałęzi na żywo.</span><span class="sxs-lookup"><span data-stu-id="97927-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="97927-124">Następnie przejdź do [portalu partnera Alchemy](https://alchemyportal.azurewebsites.net) i wprowadź nazwę pliku w polu URL.</span><span class="sxs-lookup"><span data-stu-id="97927-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 
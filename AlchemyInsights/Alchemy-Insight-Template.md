---
title: tak samo jak nazwa pliku jest najlepsza
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750980"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="f30e5-102">"Wymagany nagłówek Alchemii H1, H2 nie działa."</span><span class="sxs-lookup"><span data-stu-id="f30e5-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="f30e5-103">Najlepsze praktyki i wytyczne dotyczące tworzenia alchemii:</span><span class="sxs-lookup"><span data-stu-id="f30e5-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="f30e5-104">**Nie zagnieżdżaj Alchemy Insights w folderach**- spowoduje to przerwanie struktury adresów URL.</span><span class="sxs-lookup"><span data-stu-id="f30e5-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="f30e5-105">Szukamy rozwiązania tego problemu.</span><span class="sxs-lookup"><span data-stu-id="f30e5-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="f30e5-106">Pliki w folderze **AlchemyInsights** powinny zawierać małe nazwy plików z myślnikami dla spacji ex.</span><span class="sxs-lookup"><span data-stu-id="f30e5-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="f30e5-107">***how-to-enable-litigation-hold***.</span><span class="sxs-lookup"><span data-stu-id="f30e5-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="f30e5-108">W polu ms.custom należy uwzględnić identyfikator reguły lub identyfikator zasobnika z [portalu partnera alchemii.](https://alchemyportal.azurewebsites.net)</span><span class="sxs-lookup"><span data-stu-id="f30e5-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="f30e5-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="f30e5-109">ex.</span></span> <span data-ttu-id="f30e5-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="f30e5-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="f30e5-111">Użyj pozostałych metadanych w górnej części tego pliku jako szablonu.</span><span class="sxs-lookup"><span data-stu-id="f30e5-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="f30e5-112">W [portalu Alchemy Partner](https://alchemyportal.azurewebsites.net)przejdź do sekcji **Customer Insight Title:** i użyj tego jako punktu wyjścia dla swojego tytułu H1, aby uzyskać wgląd.</span><span class="sxs-lookup"><span data-stu-id="f30e5-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="f30e5-113">Alchemy Insights musi mieć tylko jeden H1 na górze lub będą one przerwy w produkcji.</span><span class="sxs-lookup"><span data-stu-id="f30e5-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="f30e5-114">H2s nie renderują tak używać **pogrubienia** lub innych konwencji, aby oznaczać oddzielne sekcje.</span><span class="sxs-lookup"><span data-stu-id="f30e5-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="f30e5-115">Następnie wypełnij tekst podstawowy, korzystając z projektu materiału w sekcji Customer Insights na stronie Reguła alchemii</span><span class="sxs-lookup"><span data-stu-id="f30e5-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="f30e5-116">Listy punktowane są w porządku</span><span class="sxs-lookup"><span data-stu-id="f30e5-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="f30e5-117">Ponumerowane listy też</span><span class="sxs-lookup"><span data-stu-id="f30e5-117">Numbered lists too</span></span>
    1. <span data-ttu-id="f30e5-118">**Pogrubienie** i *kursywa* są ok</span><span class="sxs-lookup"><span data-stu-id="f30e5-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="f30e5-119">Linki powinny być zawsze **albo "linki do sieci"/ zewnętrzne** lub **głębokie linki do elementów interfejsu użytkownika,** a nie linki wewnętrzne.</span><span class="sxs-lookup"><span data-stu-id="f30e5-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="f30e5-120">Zdjęcia nie są oficjalnie obsługiwane w tej chwili, ale jest na mapie drogowej.</span><span class="sxs-lookup"><span data-stu-id="f30e5-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="f30e5-121">I to jest naprawdę już trochę za długo.</span><span class="sxs-lookup"><span data-stu-id="f30e5-121">And this is really already a bit too long.</span></span> <span data-ttu-id="f30e5-122">Najlepszą praktyką jest około 400 znaków ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="f30e5-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="f30e5-123">Gdy zawartość będzie gotowa, przeciągnij ją do gałęzi na żywo.</span><span class="sxs-lookup"><span data-stu-id="f30e5-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="f30e5-124">Następnie przejdź do [portalu Partner Alchemy](https://alchemyportal.azurewebsites.net) i wprowadź nazwę pliku w polu adresu URL.</span><span class="sxs-lookup"><span data-stu-id="f30e5-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 
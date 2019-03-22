---
title: najlepiej jest sama, jak nazwa pliku
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 5555
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 68f743ee9c448565470815f8410cc6ce4b384bed
ms.sourcegitcommit: 0b6e9470c6b73616ba8bacef7010f739b7fac332
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/21/2019
ms.locfileid: "30742438"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="cca37-102">Wymagane Alchemy nagłówka H1, H2's nie działają.</span><span class="sxs-lookup"><span data-stu-id="cca37-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="cca37-103">Najważniejsze wskazówki i wytyczne dotyczące opracowywania Alchemy:</span><span class="sxs-lookup"><span data-stu-id="cca37-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="cca37-104">**Nie zagnieżdżaj spostrzeżenia Alchemia w folderach**- spowoduje to uszkodzenie struktury adresu url.</span><span class="sxs-lookup"><span data-stu-id="cca37-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="cca37-105">Pracujemy nad rozwiązaniem naprawienie tego.</span><span class="sxs-lookup"><span data-stu-id="cca37-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="cca37-106">Pliki w folderze **AlchemyInsights** powinny mieć małe litery nazw plików z łączniki do spacji, np.</span><span class="sxs-lookup"><span data-stu-id="cca37-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="cca37-107">***jak-to-enable sądowym***.</span><span class="sxs-lookup"><span data-stu-id="cca37-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="cca37-108">Zawierać identyfikator identyfikator reguły lub Wiadro z [portalu partnerów Alchemia](https://alchemyportal.azurewebsites.net) w polu ms.custom.</span><span class="sxs-lookup"><span data-stu-id="cca37-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="cca37-109">ex.</span><span class="sxs-lookup"><span data-stu-id="cca37-109">ex.</span></span> <span data-ttu-id="cca37-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="cca37-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="cca37-111">Wykonaj pozostałe metadanych w górnej części tego pliku jako szablonu.</span><span class="sxs-lookup"><span data-stu-id="cca37-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="cca37-112">W [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net), przejdź do sekcji **Tytuł wgląd klienta:** i wykorzystania, że jako początkowy punkt H1 tytuł za wgląd.</span><span class="sxs-lookup"><span data-stu-id="cca37-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="cca37-113">Alchemy spostrzeżeń musi mieć tylko jeden H1 u góry lub będą przerwy w produkcji.</span><span class="sxs-lookup"><span data-stu-id="cca37-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="cca37-114">H2s nie renderować tak użyj **pogrubienia** lub inne konwencje wyznaczać oddzielnych sekcjach.</span><span class="sxs-lookup"><span data-stu-id="cca37-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="cca37-115">Następnie podaj treść przy użyciu materiału wersję roboczą w sekcji analiz klienta strona reguły Alchemy</span><span class="sxs-lookup"><span data-stu-id="cca37-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="cca37-116">Listy punktowane są w porządku</span><span class="sxs-lookup"><span data-stu-id="cca37-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="cca37-117">Listy numerowane zbyt</span><span class="sxs-lookup"><span data-stu-id="cca37-117">Numbered lists too</span></span>
    1. <span data-ttu-id="cca37-118">**Pogrubienie** i *Kursywa* są OK-</span><span class="sxs-lookup"><span data-stu-id="cca37-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="cca37-119">Łącza zawsze powinna być **"łącza do sieci web" / zewnętrzne** OR **deep łącza do elementów interfejsu użytkownika**, nie wewnętrzne powiązania.</span><span class="sxs-lookup"><span data-stu-id="cca37-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="cca37-120">Obrazy nie są oficjalnie obsługiwane w tej chwili, ale jest na jego temat.</span><span class="sxs-lookup"><span data-stu-id="cca37-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="cca37-121">I jest to naprawdę już nieco zbyt długo.</span><span class="sxs-lookup"><span data-stu-id="cca37-121">And this is really already a bit too long.</span></span> <span data-ttu-id="cca37-122">Najlepszym rozwiązaniem jest około 400 znaków---</span><span class="sxs-lookup"><span data-stu-id="cca37-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="cca37-123">Zawartość jest gotowy, należy przeciągnąć ją do gałęzi na żywo.</span><span class="sxs-lookup"><span data-stu-id="cca37-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="cca37-124">Następnie przejdź do [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net) i wprowadź nazwę pliku w polu adres url.</span><span class="sxs-lookup"><span data-stu-id="cca37-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="cca37-125">M</span><span class="sxs-lookup"><span data-stu-id="cca37-125">M</span></span>
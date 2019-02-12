---
title: 'tak samo jak najlepiej nazwa_pliku [reguła #-opis]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939311"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="7539b-102">Wymagane Alchemy nagłówka H1, H2's nie działają.</span><span class="sxs-lookup"><span data-stu-id="7539b-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="7539b-103">Najważniejsze wskazówki i wytyczne dotyczące opracowywania Alchemy:</span><span class="sxs-lookup"><span data-stu-id="7539b-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="7539b-p101">**Nie zagnieżdżaj spostrzeżenia Alchemia w folderach**- spowoduje to uszkodzenie struktury adresu url. Pracujemy nad rozwiązaniem naprawienie tego.</span><span class="sxs-lookup"><span data-stu-id="7539b-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="7539b-106">Pliki w folderze **AlchemyInsights** powinny mieć identyfikator reguły i nazwa reguły z [portalu partnerów Alchemia](https://alchemyportal.azurewebsites.net) w nazwie pliku.</span><span class="sxs-lookup"><span data-stu-id="7539b-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="7539b-p102">ex. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="7539b-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="7539b-p103">Użyj metadanych w górnej części tego pliku jako szablonu. Nic innego nie jest wymagane.</span><span class="sxs-lookup"><span data-stu-id="7539b-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="7539b-111">W [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net), przejdź do sekcji **Tytuł wgląd klienta:** i wykorzystania, że jako początkowy punkt H1 tytuł za wgląd.</span><span class="sxs-lookup"><span data-stu-id="7539b-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="7539b-p104">Alchemy spostrzeżeń musi mieć tylko jeden H1 u góry lub będą przerwy w produkcji. H2s nie renderować tak użyj **pogrubienia** lub inne konwencje wyznaczać oddzielnych sekcjach.</span><span class="sxs-lookup"><span data-stu-id="7539b-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="7539b-114">Następnie podaj treść przy użyciu materiału wersję roboczą w sekcji analiz klienta strona reguły Alchemy</span><span class="sxs-lookup"><span data-stu-id="7539b-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="7539b-115">Listy punktowane są w porządku</span><span class="sxs-lookup"><span data-stu-id="7539b-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="7539b-116">Listy numerowane zbyt</span><span class="sxs-lookup"><span data-stu-id="7539b-116">Numbered lists too</span></span>
    1. <span data-ttu-id="7539b-117">**Pogrubienie** i *Kursywa* są OK-</span><span class="sxs-lookup"><span data-stu-id="7539b-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="7539b-118">Łącza zawsze powinna być **"łącza do sieci web" / zewnętrzne** OR **deep łącza do elementów interfejsu użytkownika**, nie wewnętrzne powiązania.</span><span class="sxs-lookup"><span data-stu-id="7539b-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="7539b-p105">I jest to naprawdę już nieco zbyt długo. Najlepszym rozwiązaniem jest około 400 znaków---</span><span class="sxs-lookup"><span data-stu-id="7539b-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="7539b-p106">Zawartość jest gotowy, należy przeciągnąć ją do gałęzi na żywo. Następnie przejdź do [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net) i wprowadź nazwę pliku w polu adres url. Upewnij się, Insight przeglądowi i opublikowane mówi "tak", a następnie kliknij regułę aktualizacji. **(To będą wyglądały w nowej wersji portalu - zwolnienie wkrótce.)** 
 ![pole adresu url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="7539b-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>


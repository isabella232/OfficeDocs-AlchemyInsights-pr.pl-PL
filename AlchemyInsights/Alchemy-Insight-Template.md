---
title: Ta sama nazwa pliku jest Najlepsza
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664144"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="2a045-102">"Wymagany nagłówek Alchemy H1, H2's nie działa".</span><span class="sxs-lookup"><span data-stu-id="2a045-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="2a045-103">Najważniejsze wskazówki i wskazówki dotyczące tworzenia Alchemy:</span><span class="sxs-lookup"><span data-stu-id="2a045-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="2a045-104">**Nie Zagnieżdżaj Alchemy w folderach**— spowoduje to zerwanie struktury adresu URL.</span><span class="sxs-lookup"><span data-stu-id="2a045-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="2a045-105">Szukamy tego rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="2a045-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="2a045-106">Pliki w folderze **AlchemyInsights** powinny zawierać małe nazwy plików z łącznikami dla spacji.</span><span class="sxs-lookup"><span data-stu-id="2a045-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="2a045-107">***jak włączyć-to***-wymuszanie — zawieszone.</span><span class="sxs-lookup"><span data-stu-id="2a045-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="2a045-108">Dołącz Identyfikator reguły lub identyfikator zasobnika z [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net) w polu MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="2a045-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="2a045-109">statek.</span><span class="sxs-lookup"><span data-stu-id="2a045-109">ex.</span></span> <span data-ttu-id="2a045-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="2a045-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="2a045-111">Użyj pozostałych metadanych u góry tego pliku jako szablonu.</span><span class="sxs-lookup"><span data-stu-id="2a045-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="2a045-112">W [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net)przejdź w dół do sekcji **zatytułowanej szczegółowy tytuł klienta:** i Użyj tej wartości jako punktu początkowego tytułu H1 do wglądu.</span><span class="sxs-lookup"><span data-stu-id="2a045-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="2a045-113">Wyniki Alchemy muszą mieć tylko jeden H1 u początku lub mogą się one pojawić w trakcie produkcji.</span><span class="sxs-lookup"><span data-stu-id="2a045-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="2a045-114">H2s nie renderowanie w ten sposób używania **pogrubienia** i innych konwencji do oznaczania odrębnych sekcji.</span><span class="sxs-lookup"><span data-stu-id="2a045-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="2a045-115">Następnie wypełnij tekst podstawowy za pomocą wersji roboczej materiałów dostępnych w sekcji Informacje o klientach na stronie reguły Alchemy</span><span class="sxs-lookup"><span data-stu-id="2a045-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="2a045-116">Listy punktowane są bardzo cienkie</span><span class="sxs-lookup"><span data-stu-id="2a045-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="2a045-117">Listy numerowane są też</span><span class="sxs-lookup"><span data-stu-id="2a045-117">Numbered lists too</span></span>
    1. <span data-ttu-id="2a045-118">**Pogrubienie** i *kursywa* to a-OK</span><span class="sxs-lookup"><span data-stu-id="2a045-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="2a045-119">Linki powinny być zawsze **"linkami do sieci Web"/External** lub **głębokie linki do elementów interfejsu użytkownika**, a nie łączami wewnętrznymi.</span><span class="sxs-lookup"><span data-stu-id="2a045-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="2a045-120">Obrazy nie są obecnie obsługiwane w tym czasie, ale są na mapie.</span><span class="sxs-lookup"><span data-stu-id="2a045-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="2a045-121">Jest to naprawdę już zbyt długi.</span><span class="sxs-lookup"><span data-stu-id="2a045-121">And this is really already a bit too long.</span></span> <span data-ttu-id="2a045-122">Najlepsza praktyka dotyczy około 400 znaków---------------------------------</span><span class="sxs-lookup"><span data-stu-id="2a045-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="2a045-123">Gdy zawartość będzie gotowa, pociągnij ją do gałęzi na żywo.</span><span class="sxs-lookup"><span data-stu-id="2a045-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="2a045-124">Następnie przejdź do [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net) i wprowadź nazwę pliku w polu adres URL.</span><span class="sxs-lookup"><span data-stu-id="2a045-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 
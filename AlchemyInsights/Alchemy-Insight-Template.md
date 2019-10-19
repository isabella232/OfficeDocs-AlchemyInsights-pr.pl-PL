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
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Wymagane Alchemy header H1, H2 nie działają.
Sprawdzone metody i wskazówki dotyczące tworzenia treści Alchemy:

1. **Nie zagnieżdżać Alchemy Insights w folderach**-spowoduje to przerwanie struktury URL. Patrzymy na naprawienie tego.
1. Pliki w folderze **Alchemyinsights** powinny mieć małe nazwy plików z myślkami dla spacji ex. ***jak-wobec-umożliwiać-sądowym-Hold***.
    1. Dołącz Identyfikator reguły lub identyfikator zasobnika z [portalu partnera Alchemy](https://alchemyportal.azurewebsites.net) w polu MS. Custom. Ex. ***MS. zwyczaj: 100021***
1. Użyj pozostałej części metadanych w górnej części tego pliku jako szablonu.
1. W [portalu dla partnerów Alchemy](https://alchemyportal.azurewebsites.net)przejdź w dół do sekcji **Customer Insight title:** i wykorzystaj to jako punkt wyjścia dla swojego tytułu H1 dla wglądu. 
    > [!NOTE]
    > Alchemy Insights musi mieć tylko jeden H1 na górze lub będą one złamać w produkcji. H2s nie renderuje tak więc Użyj **pogrubienie** lub inne konwencje oznaczają oddzielne sekcje.
1. Następnie wypełnij tekst treści za pomocą materiałów roboczych w sekcji Customer Insights na stronie reguła alchemii.
    1. Listy wypunktowane są w porządku
    1. Listy numerowane zbyt
    1. **Pogrubienie** i *kursywa* są-OK
    1. Łącza zawsze powinny być albo **"łącza do sieci Web"/External** lub **Deep-łącza do elementów interfejsu użytkownika**, a nie wewnętrzne łącza.
    1. Zdjęcia nie są oficjalnie wspierane w tej chwili, ale to na planie.

I to jest naprawdę już trochę za długo. Najlepsze praktyki jest około 400 znaków---------------------------------

Gdy zawartość będzie gotowa, pociągnij ją do gałęzi na żywo. Następnie przejdź do [portalu partnera Alchemy](https://alchemyportal.azurewebsites.net) i wprowadź nazwę pliku w polu URL. 
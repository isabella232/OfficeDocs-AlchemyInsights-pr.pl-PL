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
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Wymagany nagłówek Alchemii H1, H2 nie działa."
Najlepsze praktyki i wytyczne dotyczące tworzenia alchemii:

1. **Nie zagnieżdżaj Alchemy Insights w folderach**- spowoduje to przerwanie struktury adresów URL. Szukamy rozwiązania tego problemu.
1. Pliki w folderze **AlchemyInsights** powinny zawierać małe nazwy plików z myślnikami dla spacji ex. ***how-to-enable-litigation-hold***.
    1. W polu ms.custom należy uwzględnić identyfikator reguły lub identyfikator zasobnika z [portalu partnera alchemii.](https://alchemyportal.azurewebsites.net) Ex. ***ms.custom: 100021***
1. Użyj pozostałych metadanych w górnej części tego pliku jako szablonu.
1. W [portalu Alchemy Partner](https://alchemyportal.azurewebsites.net)przejdź do sekcji **Customer Insight Title:** i użyj tego jako punktu wyjścia dla swojego tytułu H1, aby uzyskać wgląd. 
    > [!NOTE]
    > Alchemy Insights musi mieć tylko jeden H1 na górze lub będą one przerwy w produkcji. H2s nie renderują tak używać **pogrubienia** lub innych konwencji, aby oznaczać oddzielne sekcje.
1. Następnie wypełnij tekst podstawowy, korzystając z projektu materiału w sekcji Customer Insights na stronie Reguła alchemii
    1. Listy punktowane są w porządku
    1. Ponumerowane listy też
    1. **Pogrubienie** i *kursywa* są ok
    1. Linki powinny być zawsze **albo "linki do sieci"/ zewnętrzne** lub **głębokie linki do elementów interfejsu użytkownika,** a nie linki wewnętrzne.
    1. Zdjęcia nie są oficjalnie obsługiwane w tej chwili, ale jest na mapie drogowej.

I to jest naprawdę już trochę za długo. Najlepszą praktyką jest około 400 znaków ---------------------------------

Gdy zawartość będzie gotowa, przeciągnij ją do gałęzi na żywo. Następnie przejdź do [portalu Partner Alchemy](https://alchemyportal.azurewebsites.net) i wprowadź nazwę pliku w polu adresu URL. 
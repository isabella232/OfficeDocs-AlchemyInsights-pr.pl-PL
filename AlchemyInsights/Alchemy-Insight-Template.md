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
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30762074"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Wymagane Alchemy nagłówka H1, H2's nie działają.
Najważniejsze wskazówki i wytyczne dotyczące opracowywania Alchemy:

1. **Nie zagnieżdżaj spostrzeżenia Alchemia w folderach**- spowoduje to uszkodzenie struktury adresu url. Pracujemy nad rozwiązaniem naprawienie tego.
1. Pliki w folderze **AlchemyInsights** powinny mieć małe litery nazw plików z łączniki do spacji, np. ***jak-to-enable sądowym***.
    1. Zawierać identyfikator identyfikator reguły lub Wiadro z [portalu partnerów Alchemia](https://alchemyportal.azurewebsites.net) w polu ms.custom. ex. ***MS.Custom: 100021***
1. Wykonaj pozostałe metadanych w górnej części tego pliku jako szablonu.
1. W [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net), przejdź do sekcji **Tytuł wgląd klienta:** i wykorzystania, że jako początkowy punkt H1 tytuł za wgląd. 
    > [!NOTE]
    > Alchemy spostrzeżeń musi mieć tylko jeden H1 u góry lub będą przerwy w produkcji. H2s nie renderować tak użyj **pogrubienia** lub inne konwencje wyznaczać oddzielnych sekcjach.
1. Następnie podaj treść przy użyciu materiału wersję roboczą w sekcji analiz klienta strona reguły Alchemy
    1. Listy punktowane są w porządku
    1. Listy numerowane zbyt
    1. **Pogrubienie** i *Kursywa* są OK-
    1. Łącza zawsze powinna być **"łącza do sieci web" / zewnętrzne** OR **deep łącza do elementów interfejsu użytkownika**, nie wewnętrzne powiązania.
    1. Obrazy nie są oficjalnie obsługiwane w tej chwili, ale jest na jego temat.

I jest to naprawdę już nieco zbyt długo. Najlepszym rozwiązaniem jest około 400 znaków---

Zawartość jest gotowy, należy przeciągnąć ją do gałęzi na żywo. Następnie przejdź do [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net) i wprowadź nazwę pliku w polu adres url. M
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
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Wymagane Alchemy nagłówka H1, H2's nie działają.
Najważniejsze wskazówki i wytyczne dotyczące opracowywania Alchemy:

1. **Nie zagnieżdżaj spostrzeżenia Alchemia w folderach**- spowoduje to uszkodzenie struktury adresu url. Pracujemy nad rozwiązaniem naprawienie tego.
1. Pliki w folderze **AlchemyInsights** powinny mieć identyfikator reguły i nazwa reguły z [portalu partnerów Alchemia](https://alchemyportal.azurewebsites.net) w nazwie pliku.
    1. ex. ***976-How-to-enable-litigation-hold***
1. Użyj metadanych w górnej części tego pliku jako szablonu. Nic innego nie jest wymagane.
1. W [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net), przejdź do sekcji **Tytuł wgląd klienta:** i wykorzystania, że jako początkowy punkt H1 tytuł za wgląd. 
    > [!NOTE]
    > Alchemy spostrzeżeń musi mieć tylko jeden H1 u góry lub będą przerwy w produkcji. H2s nie renderować tak użyj **pogrubienia** lub inne konwencje wyznaczać oddzielnych sekcjach.
1. Następnie podaj treść przy użyciu materiału wersję roboczą w sekcji analiz klienta strona reguły Alchemy
    1. Listy punktowane są w porządku
    1. Listy numerowane zbyt
    1. **Pogrubienie** i *Kursywa* są OK-
    1. Łącza zawsze powinna być **"łącza do sieci web" / zewnętrzne** OR **deep łącza do elementów interfejsu użytkownika**, nie wewnętrzne powiązania.

I jest to naprawdę już nieco zbyt długo. Najlepszym rozwiązaniem jest około 400 znaków---

Zawartość jest gotowy, należy przeciągnąć ją do gałęzi na żywo. Następnie przejdź do [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net) i wprowadź nazwę pliku w polu adres url. Upewnij się, Insight przeglądowi i opublikowane mówi "tak", a następnie kliknij regułę aktualizacji. **(To będą wyglądały w nowej wersji portalu - zwolnienie wkrótce.)** 
 ![pole adresu url](media/for-content-team.PNG)


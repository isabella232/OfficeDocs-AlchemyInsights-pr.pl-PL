---
title: najlepsze jest to, co jest takie samo, jak nazwa pliku
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
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312835"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Wymagany nagłówek Alchemy H1, nie działa H2".
Najlepsze rozwiązania i wskazówki dotyczące tworzenia Alchemy:

1. **Nie zagnieżdżaj alchemy Szczegółowe informacje folderach**— spowoduje to zerwanie struktury adresu URL. Pracujemy nad rozwiązaniem tego problemu.
1. Pliki w **folderze AlchemyInsights** powinny mieć małe nazwy plików z łącznikami, na przykład spacje. **_how-to-enable-litigation-hold._**
    1. Dołącz identyfikator reguły lub identyfikator zasobnika z [portalu partnera Alchemy w](https://alchemyportal.azurewebsites.net) polu ms.custom. np. ***ms.custom: 100021***
1. Użyj pozostałych metadanych w górnej części tego pliku jako szablonu.
1. W portalu [partnerów Alchemy](https://alchemyportal.azurewebsites.net)przejdź do sekcji Tytuł informacji o klientach **i** użyj jej jako punktu wyjścia dla tytułu H1. 

**Uwaga:** Alchemy Szczegółowe informacje MUSI mieć u góry tylko jeden H1, aby nie został wyłamyny w produkcji. H2 nie są renderowane, dlatego użyj pogrubienia **lub** innych konwencji, aby oznaczać osobne sekcje.
1. Następnie wypełnij tekst treści przy użyciu materiału roboczego w sekcji Customer Insights sekcji Reguła Alchemy'ego
    1. Listy punktowane są w porządku
    1. Również listy numerowane
    1. **Pogrubienie** *i kursywa* są ok
    1. Linki powinny zawsze być **"linkami do sieci Web"/zewnętrznymi** LUB **deep-linksami** do elementów interfejsu użytkownika, a nie linkami wewnętrznymi.
    1. Obecnie obrazy nie są oficjalnie obsługiwane, ale są w planach.

A to jest naprawdę trochę za długo. Najlepsze rozwiązanie to około 400 znaków ---------------------------------

Gdy zawartość będzie gotowa, pociągnij ją do gałęzi na żywo. Następnie przejdź do portalu [partnera Alchemy i](https://alchemyportal.azurewebsites.net) wprowadź nazwę pliku w polu adresu URL. 
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
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918905"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Wymagany nagłówek Alchemy H1, nie działa H2".
Najlepsze rozwiązania i wskazówki dotyczące tworzenia Alchemy:

1. **Nie zagnieżdżaj alchemy Szczegółowe informacje folderach**— spowoduje to zerwanie struktury adresu URL. Pracujemy nad rozwiązaniem tego problemu.
1. Pliki w **folderze AlchemyInsights** powinny mieć małe nazwy plików z łącznikami, na przykład spacje. **_how-to-enable-litigation-hold._**
    1. Dołącz identyfikator reguły lub identyfikator zasobnika z [portalu partnera Alchemy w](https://alchemyportal.azurewebsites.net) polu ms.custom. np. ***ms.custom: 100021***
1. Użyj pozostałych metadanych w górnej części tego pliku jako szablonu.
1. W portalu [partnerów Alchemy](https://alchemyportal.azurewebsites.net)przejdź do sekcji Tytuł informacji o klientach **i** użyj jej jako punktu wyjścia dla tytułu H1. 
    > [!NOTE]
    > Alchemy Szczegółowe informacje ŻE U góry MUSI znajdować się tylko jeden H1, aby w końcu zostały one wyrywne w produkcji. H2 nie są renderowane, dlatego użyj pogrubienia **lub** innych konwencji, aby oznaczać osobne sekcje.
1. Następnie wypełnij tekst treści za pomocą materiału roboczego w sekcji Customer Insights artykułu na stronie Reguła Alchemy'ego
    1. Listy punktowane są w porządku
    1. Również listy numerowane
    1. **Pogrubienie** *i kursywa* są ok
    1. Linki powinny zawsze być **"linkami do sieci Web"/zewnętrznymi** LUB wewnętrznymi linkami do elementów **interfejsu** użytkownika, a nie linkami wewnętrznymi.
    1. Obecnie obrazy nie są oficjalnie obsługiwane, ale są w planach.

A to jest naprawdę trochę za długo. Najlepsze rozwiązanie to około 400 znaków w ---------------------------------

Gdy zawartość będzie gotowa, pociągnij ją do gałęzi na żywo. Następnie przejdź do portalu [partnera Alchemy i](https://alchemyportal.azurewebsites.net) wprowadź nazwę pliku w polu adresu URL. 
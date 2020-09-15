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
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Wymagany nagłówek Alchemy H1, H2's nie działa".
Najważniejsze wskazówki i wskazówki dotyczące tworzenia Alchemy:

1. **Nie Zagnieżdżaj Alchemy w folderach**— spowoduje to zerwanie struktury adresu URL. Szukamy tego rozwiązania.
1. Pliki w folderze **AlchemyInsights** powinny zawierać małe nazwy plików z łącznikami dla spacji. ***jak włączyć-to***-wymuszanie — zawieszone.
    1. Dołącz Identyfikator reguły lub identyfikator zasobnika z [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net) w polu MS. Custom. statek. ***MS. Custom: 100021***
1. Użyj pozostałych metadanych u góry tego pliku jako szablonu.
1. W [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net)przejdź w dół do sekcji **zatytułowanej szczegółowy tytuł klienta:** i Użyj tej wartości jako punktu początkowego tytułu H1 do wglądu. 
    > [!NOTE]
    > Wyniki Alchemy muszą mieć tylko jeden H1 u początku lub mogą się one pojawić w trakcie produkcji. H2s nie renderowanie w ten sposób używania **pogrubienia** i innych konwencji do oznaczania odrębnych sekcji.
1. Następnie wypełnij tekst podstawowy za pomocą wersji roboczej materiałów dostępnych w sekcji Informacje o klientach na stronie reguły Alchemy
    1. Listy punktowane są bardzo cienkie
    1. Listy numerowane są też
    1. **Pogrubienie** i *kursywa* to a-OK
    1. Linki powinny być zawsze **"linkami do sieci Web"/External** lub **głębokie linki do elementów interfejsu użytkownika**, a nie łączami wewnętrznymi.
    1. Obrazy nie są obecnie obsługiwane w tym czasie, ale są na mapie.

Jest to naprawdę już zbyt długi. Najlepsza praktyka dotyczy około 400 znaków---------------------------------

Gdy zawartość będzie gotowa, pociągnij ją do gałęzi na żywo. Następnie przejdź do [portalu partnerów Alchemy](https://alchemyportal.azurewebsites.net) i wprowadź nazwę pliku w polu adres URL. 
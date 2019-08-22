---
title: Wyszukaj w trybie Online w programie SharePoint
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507641"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Zawartości przeszukiwania i indeksowania w dokumentacji Online programu SharePoint

Zawartość musi przeszukanych i dodane do indeksu wyszukiwania użytkownikom znajdowanie, czego szukają w dokumentacji Online programu SharePoint. Automatycznie przeszukiwania zawartości oparty na harmonogram przeszukiwania wstępnie zdefiniowane (nie można zmienić harmonogram przeszukiwania). Przeszukiwarka odbierze zawartość, która została zmieniona od czasu ostatniego przeszukiwania i aktualizuje indeks. Aby zapewnić przeszukiwania zawartości i aktualizacji indeksu, należy zauważyć, że:

- Upewnij się, że zawartość znajduje się poprzez [przeszukiwanie zawartości witryny](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Po zmianie właściwości zarządzanej lub po zmianie mapowanie przeszukany i zarządzane właściwości witryny musi być przeszukane ponownie, zanim wprowadzone zmiany zostaną odzwierciedlone w indeksie wyszukiwania. 

    Ponieważ Twoje zmiany zostaną wprowadzone w schematu wyszukiwania, a nie do rzeczywistej witryny przeszukiwarka nie zostaną automatycznie ponowne indeksowanie witryny. 

    Aby uzyskać więcej informacji zobacz temat [ręcznie zażądać i ponownego indeksowania danej witryny, listy lub biblioteki](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Odczekaj co najmniej 24 godziny po zażądaniu ręcznie przeszukiwania i pełne ponowne indeksowanie aby zobaczyć, czy nadal występują problemu. 

    Jeśli więcej niż 24 godziny upłynęło od momentu zainicjowania przeszukiwania i pełne ponowne indeksowanie, należy zalogować się przypadek pomocy technicznej. W wielu przypadkach już pracujemy nad rozwiązaniem. Podaj co najmniej 24 godziny, aby ukończyć rozwiązania.

> [!IMPORTANT]
> Jeśli witryna, dokument (Biblioteka) lub listę został usunięty i nadal wyświetlany w wynikach wyszukiwania, użytkownik powinien otrzymać **Błąd 404 Nie można odnaleźć pliku** podczas próby dostępu do niego. Ten problem powinny być rejestrowane jako przypadek pomocy technicznej w odniesieniu do dalszych badań. 




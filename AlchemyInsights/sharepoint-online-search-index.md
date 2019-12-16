---
title: Wyszukiwanie w programie SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044053"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Indeksowanie zawartości i indeksowania w programie SharePoint Online

Zawartość musi być przeszukiwany i dodawany do indeksu wyszukiwania dla użytkowników, aby znaleźć to, czego szukają w programie SharePoint Online. Zawartość jest automatycznie przeszukiwany na podstawie wstępnie zdefiniowanego harmonogramu przeszukiwania (nie można zmienić harmonogramu przeszukiwania). Przeszukiwarka przejmuje zawartość, która zmieniła się od czasu ostatniego przeszukiwania i aktualizuje indeks. Aby upewnić się, że zawartość jest przeszukowana, a indeks jest aktualizowany, należy zwrócić uwagę na następujące elementy:

- Upewnij się, że zawartość może zostać znaleziona poprzez [przeszukanie zawartości witryny](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Po zmianie właściwości zarządzanej lub zmianie mapowania właściwości przeszukanych i zarządzanych lokacja musi zostać ponownie przeszukana, zanim zmiany zostaną odzwierciedlone w indeksie wyszukiwania. 

    Ponieważ zmiany są wprowadzane w schemacie wyszukiwania, a nie do rzeczywistej witryny, przeszukiwarka nie będzie automatycznie ponownie indeksować witryny. 

    Aby uzyskać więcej informacji, zobacz [Ręczne żądanie indeksowania i ponownego indeksowania witryny, biblioteki lub listy](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Poczekaj co najmniej 24 godziny po ręcznym zażądaniu indeksowania i pełnego ponownego indeksowania, aby sprawdzić, czy nadal występuje problem. 

    Jeśli upłynęło więcej niż 24 godziny od zainicjowania indeksowania i pełnego ponownego indeksowania, należy zalogować się w przypadku pomocy technicznej. W wielu przypadkach pracujemy już nad rozwiązaniem. Proszę dać nam co najmniej 24 godziny, aby zakończyć rozwiązanie.

> [!IMPORTANT]
> Jeśli witryna, dokument (Biblioteka) lub lista zostały usunięte i nadal są wyświetlane w wynikach wyszukiwania, użytkownicy powinni otrzymać **błąd 404 nie można odnaleźć pliku** podczas próby uzyskania do niego dostępu. Ten problem powinien być rejestrowane jako przypadek pomocy technicznej do dalszego dochodzenia. 




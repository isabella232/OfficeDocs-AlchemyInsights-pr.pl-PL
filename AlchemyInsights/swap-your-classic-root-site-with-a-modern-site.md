---
title: Zamiana klasycznej witryny głównej na nowoczesną witrynę
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316150"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamiana klasycznej witryny głównej na nowoczesną witrynę

Jeśli Twoje środowisko zostało skonfigurować przed kwietniem 2019 r., możesz zmienić witrynę główną w nowoczesną za pomocą programu Microsoft PowerShell:

- Jeśli jako witryny głównej chcesz użyć innej witryny, możesz zamienić [witrynę](https://docs.microsoft.com/sharepoint/modern-root-site) główną (zamienić ją na inną). 
    - Użyj [funkcji Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) aby zamienić lokalizację witryny z inną witryną podczas archiwizowania pierwotnej witryny. Dostępne zarówno dla witryny zespołu (nie połączonej z grupą), jak i dla witryny do komunikacji. 

- Wkrótce zostaną wprowadzone dodatkowe funkcje, które umożliwią nadal korzystanie z zawartości witryny, ale przekonwertowanie istniejącej witryny na witrynę do komunikacji. 

**Ważne:** te funkcje będą stopniowo rozszerzane. Sprawdź aktualizacje w Centrum wiadomości. 

## <a name="known-issues-with-swapping-sites"></a>Znane problemy dotyczące zamieniania witryn

- W witrynie docelowej przez krótki czas może zostać zwrócony błąd "nie znaleziono" (HTTP 404).
- Aby zaktualizować indeks wyszukiwania, należy ponownie zaktualizować zawartość. Nie trzeba ręcznie nic robić — zostanie to zrobione automatycznie.
- Wszystko, co zależy od "statycznych" linków (takich jak synchronizacja plików i pliki OneNote) trzeba będzie poprawić ręcznie.
- Jeśli witryna źródłowa była witryną wiadomości organizacji, zaktualizuj adres URL. Uzyskaj listę wszystkich witryn wiadomości organizacji.
- Project Być może trzeba sprawdzić poprawność witryn serwera, aby upewnić się, że są one nadal prawidłowo skojarzone.

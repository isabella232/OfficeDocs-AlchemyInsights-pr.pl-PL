---
title: Zamień swoją klasyczną witrynę główną na nowoczesną witrynę
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741554"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamień swoją klasyczną witrynę główną na nowoczesną witrynę

Jeśli środowisko zostało skonfigurowane przed kwietniem 2019 r., można zmienić witrynę główną na nowoczesną witrynę przy użyciu programu Microsoft PowerShell:

- Jeśli masz inną witrynę, której chcesz użyć jako witryny głównej, możesz zastąpić [ją (zamienić) witrynę główną.](https://docs.microsoft.com/sharepoint/modern-root-site) 
    - Użyj [invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) aby zamienić lokalizację lokacji z inną witryną podczas archiwizowania oryginalnej witryny. Dostępne zarówno dla witryny zespołu (niepodłączonej do grupy), jak i dla witryny komunikacyjnej. 

- Wkrótce zostaną wprowadzone dodatkowe funkcje, które pozwolą ci nadal korzystać z zawartości witryny, ale przekonwertować istniejącą witrynę na witrynę komunikacyjną. 
>[!Important]
>Możliwości te będą wprowadzane stopniowo. Kontynuuj sprawdzanie aktualizacji w Centrum wiadomości. 

## <a name="known-issues-with-swapping-sites"></a>Znane problemy z zamianą witryn

- Witryna docelowa może zwrócić błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.
- Zawartość będzie musiała zostać ponownie zindeksowana, aby zaktualizować indeks wyszukiwania. Nie jest wymagany żaden ręczny krok - zostanie to zrobione automatycznie.
- Wszystko, co zależy od "statycznych" łączy (takich jak synchronizacja plików i pliki programu OneNote) będzie musiało zostać ręcznie poprawione.
- Jeśli witryna źródłowsza była witryną wiadomości organizacji, zaktualizuj adres URL.Pobierz listę wszystkich witryn z wiadomościami organizacyjnymi.
- Witryny programu Project Server mogą wymagać sprawdzenia poprawności, aby upewnić się, że są one nadal poprawnie skojarzone.

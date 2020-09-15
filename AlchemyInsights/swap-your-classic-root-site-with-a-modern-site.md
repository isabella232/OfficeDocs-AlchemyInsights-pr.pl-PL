---
title: Zamienianie klasycznej witryny głównej na witrynę Modern
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691189"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamienianie klasycznej witryny głównej na witrynę Modern

Jeśli Twoje środowisko zostało skonfigurowane przed wydaniem 2019 kwietnia, możesz zmienić witrynę główną na witrynę Modern za pomocą programu Microsoft PowerShell:

- Jeśli masz inną witrynę, która ma być używana jako witryna główna, możesz zamienić ją [na witrynę główną (zamieniać](https://docs.microsoft.com/sharepoint/modern-root-site) się na nią). 
    - Użyj funkcji [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , aby zamienić lokalizację witryny na inną witrynę podczas archiwizacji oryginalnej witryny. Dostępne w przypadku witryny zespołu (niepołączonej z grupą) i witryny do komunikacji. 

- Zostaną wkrótce wprowadzone dodatkowe funkcje, które umożliwią korzystanie z zawartości witryny, ale Konwertowanie istniejącej witryny na witrynę komunikacyjną. 
>[!Important]
>Te funkcje zostaną stopniowo rozwijane. Kontynuuj sprawdzanie aktualizacji w centrum wiadomości. 

## <a name="known-issues-with-swapping-sites"></a>Znane problemy dotyczące wymiany witryn

- Witryna docelowa może zwracać błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.
- Aby zaktualizować indeks wyszukiwania, zawartość musi zostać przeszukana ponownie. Nie jest wymagany ręczny krok — zostanie on wykonany automatycznie.
- Wszystkie osoby zależne od linków "static" (takie jak synchronizacja plików i pliki programu OneNote) trzeba będzie ręcznie poprawić.
- Jeśli witryna źródłowa była witryną grup dyskusyjnych, zaktualizuj adres URL.Zapoznaj się z listą wszystkich witryn z informacjami organizacyjnymi.
- Witryny programu Project Server mogą wymagać sprawdzenia, aby upewnić się, że są nadal poprawnie skojarzone.

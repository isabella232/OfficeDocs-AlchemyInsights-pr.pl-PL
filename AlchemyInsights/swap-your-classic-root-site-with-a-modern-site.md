---
title: Zamień swoją stronę główną Classic z nowoczesnym miejscu
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042937"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamień swoją stronę główną Classic z nowoczesnym miejscu

Jeśli środowisko zostało skonfigurowane przed kwietniem 2019, można zmienić witryny głównej do nowoczesnej witryny przy użyciu programu Microsoft PowerShell:

- Jeśli masz inną witrynę, która ma być używany jako witryny głównej, można zastąpić [(swap) witryny głównej](https://docs.microsoft.com/sharepoint/modern-root-site) z nim. 
    - Użyj [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) do zamiany lokalizacji witryny z innej witryny podczas archiwizacji oryginalnej witryny. Dostępne zarówno dla witryny zespołu (niepołączonej z grupą), jak i witryny komunikacyjnej. 

- Wkrótce zostaną wprowadzone dodatkowe możliwości, które pozwolą na dalsze korzystanie z zawartości witryny, ale przekonwertowanie istniejącej witryny na witrynę komunikacyjną. 
>[!Important]
>Te możliwości będą wprowadzane stopniowo. Kontynuuj sprawdzanie centrum wiadomości pakietu Office 365 dla aktualizacji. 

## <a name="known-issues-with-swapping-sites"></a>Znane problemy z zamianę witryn

- Witryna docelowa może zwracać błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.
- Aby zaktualizować indeks wyszukiwania, konieczne będzie ponowne zaindeksowanie zawartości. Nie jest wymagane ręczne krok-to będzie zrobione automatycznie.
- Wszystko, co jest zależne od "statyczne" łącza (takie jak pliki synchronizacji plików i OneNote) należy ręcznie skorygować.
- Jeśli witryna źródłowa była witryną wiadomości organizacji, zaktualizuj adres URL.Uzyskaj listę wszystkich serwisów informacyjnych organizacji.
- Witryny programu Project Server może wymagać sprawdzania poprawności, aby upewnić się, że są nadal skojarzone poprawnie.






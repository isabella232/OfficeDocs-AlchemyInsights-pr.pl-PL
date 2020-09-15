---
title: Witryna Modern jako witryna główna
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666880"
---
# <a name="modern-site-as-root-site"></a>Witryna Modern jako witryna główna

Rozpoczęto wprowadzanie nowej funkcji, która umożliwi [zamianę klasycznej witryny głównej witryny na witrynę Modern](https://docs.microsoft.com/sharepoint/modern-root-site). Użyj funkcji [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , aby zamienić lokalizację witryny na inną witrynę podczas archiwizacji oryginalnej witryny. Dostępne w przypadku witryny zespołu (niepołączonej z grupą) i witryny do komunikacji.

>[!Important]
> Nie usuwaj klasycznej witryny głównej, aby utworzyć nowoczesne witryny komunikacyjne. Nie jest to obsługiwane przez firmę Microsoft. Usunięcie witryny głównej spowoduje, że we wszystkich witrynach programu SharePoint w Twojej organizacji będzie ona niedostępna do wszystkich użytkowników, do momentu przywrócenia witryny lub utworzenia nowej witryny pod tym samym adresem URL. Ta funkcja będzie przekazywana za pośrednictwem centrum wiadomości. Należy się spodziewać, że ta funkcja została wkrótce włączona w dzierżawie.

## <a name="known-issues-with-swapping-sites"></a>Znane problemy dotyczące wymiany witryn
- Witryna docelowa może zwracać błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.
- Aby zaktualizować indeks wyszukiwania, zawartość musi zostać przeszukana ponownie. W tym miejscu nie jest wymagane ręczne wykonanie tego kroku, zostanie ono automatycznie ukończone.
- Wszystkie osoby zależne od linków "static" (takie jak synchronizacja plików i pliki programu OneNote) trzeba będzie ręcznie poprawić.
- Witryny programu Project Server mogą wymagać sprawdzenia, aby upewnić się, że są nadal poprawnie skojarzone. 

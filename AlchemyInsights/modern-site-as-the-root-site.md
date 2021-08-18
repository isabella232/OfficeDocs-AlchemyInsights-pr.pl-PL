---
title: Nowoczesna witryna jako witryna główna
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
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327612"
---
# <a name="modern-site-as-root-site"></a>Nowoczesna witryna jako witryna główna

Rozpoczęliśmy prace nad rozdaniem nowej funkcji, która umożliwi zamianę klasycznej witryny głównej na [nowoczesną witrynę.](https://docs.microsoft.com/sharepoint/modern-root-site) Użyj [funkcji Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) aby zamienić lokalizację witryny z inną witryną podczas archiwizowania pierwotnej witryny. Dostępne zarówno dla witryny zespołu (nie połączonej z grupą), jak i dla witryny do komunikacji.

**Ważne:** Nie usuwaj klasycznej witryny głównej, aby utworzyć nowoczesną witrynę do komunikacji. Ta usługa nie jest obsługiwana przez firmę Microsoft. Usunięcie witryny głównej spowoduje, że SharePoint witryny w organizacji będą niedostępne dla wszystkich użytkowników, dopóki nie przywrócisz tej witryny lub nie utworzysz nowej witryny pod tym samym adresem URL. Będziemy komunikować tę funkcję za pośrednictwem Centrum wiadomości. Należy oczekiwać, że ta funkcja zostanie wkrótce włączona w dzierżawie.

## <a name="known-issues-with-swapping-sites"></a>Znane problemy dotyczące zamieniania witryn
- W witrynie docelowej przez krótki czas może zostać zwrócony błąd "nie znaleziono" (HTTP 404).
- Aby zaktualizować indeks wyszukiwania, należy ponownie zaktualizować zawartość. W tym przypadku nie jest wymagany żaden ręczny krok. Zostanie to zrobione automatycznie.
- Wszystko, co zależy od "statycznych" linków (takich jak synchronizacja plików i pliki OneNote) trzeba będzie poprawić ręcznie.
- Project Być może trzeba sprawdzić poprawność witryn serwera, aby upewnić się, że są one nadal prawidłowo skojarzone. 

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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000402"
---
# <a name="modern-site-as-root-site"></a>Nowoczesna witryna jako witryna główna

Rozpoczęliśmy prace nad rozdaniem nowej funkcji, która umożliwi zamianę klasycznej witryny głównej na [nowoczesną witrynę.](https://docs.microsoft.com/sharepoint/modern-root-site) Użyj [funkcji Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) aby zamienić lokalizację witryny z inną witryną podczas archiwizowania pierwotnej witryny. Dostępne zarówno dla witryny zespołu (nie połączonej z grupą), jak i dla witryny do komunikacji.

>[!Important]
> Nie usuwaj klasycznej witryny głównej, aby utworzyć nowoczesną witrynę do komunikacji. Ta usługa nie jest obsługiwana przez firmę Microsoft. Usunięcie witryny głównej spowoduje, że wszystkie witryny SharePoint w organizacji będą niedostępne dla wszystkich użytkowników, dopóki nie przywrócisz witryny lub nie utworzysz nowej witryny pod tym samym adresem URL. Będziemy komunikować tę funkcję za pośrednictwem Centrum wiadomości. Należy oczekiwać, że ta funkcja zostanie wkrótce włączona w dzierżawie.

## <a name="known-issues-with-swapping-sites"></a>Znane problemy dotyczące zamieniania witryn
- W witrynie docelowej przez krótki czas może zostać zwrócony błąd "nie znaleziono" (HTTP 404).
- Aby zaktualizować indeks wyszukiwania, należy ponownie zaktualizować zawartość. W tym przypadku nie jest wymagany żaden ręczny krok. Zostanie to zrobione automatycznie.
- Wszystko, co zależy od "statycznych" linków (takich jak synchronizacja plików i OneNote) będzie wymagało ręcznego poprawiania.
- Project Być może trzeba sprawdzić poprawność witryn serwera, aby upewnić się, że są one nadal prawidłowo skojarzone. 

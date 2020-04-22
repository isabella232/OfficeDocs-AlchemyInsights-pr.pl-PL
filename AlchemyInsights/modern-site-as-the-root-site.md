---
title: Nowoczesna strona jako strona główna
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713801"
---
# <a name="modern-site-as-root-site"></a>Nowoczesna strona jako strona główna

Zaczęliśmy wdrażać nową funkcję, która pozwoli Ci [zamienić klasyczną witrynę główną witryny na nowoczesną witrynę.](https://docs.microsoft.com/sharepoint/modern-root-site) Użyj [invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) aby zamienić lokalizację lokacji z inną witryną podczas archiwizowania oryginalnej witryny. Dostępne zarówno dla witryny zespołu (niepodłączonej do grupy), jak i dla witryny komunikacyjnej.

>[!Important]
> Nie usuwaj klasycznej witryny głównej, aby utworzyć nowoczesną witrynę komunikacyjną. Nie jest to obsługiwane przez firmę Microsoft. Usunięcie witryny głównej spowoduje, że wszystkie witryny programu SharePoint w organizacji staną się niedostępne dla wszystkich użytkowników, dopóki nie przywrócisz witryny lub nie utworzysz nowej witryny pod tym samym adresem URL. Będziemy komunikować tę funkcję za pośrednictwem centrum wiadomości. Należy się spodziewać, że funkcja zostanie wkrótce włączona w dzierżawie.

## <a name="known-issues-with-swapping-sites"></a>Znane problemy z zamianą witryn
- Witryna docelowa może zwrócić błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.
- Zawartość będzie musiała zostać ponownie zindeksowana, aby zaktualizować indeks wyszukiwania. Nie jest tu wymagany żaden ręczny krok, zostanie to zrobione automatycznie.
- Wszystko, co zależy od "statycznych" łączy (takich jak synchronizacja plików i pliki programu OneNote) będzie musiało zostać ręcznie poprawione.
- Witryny programu Project Server mogą wymagać sprawdzenia poprawności, aby upewnić się, że są one nadal poprawnie skojarzone. 

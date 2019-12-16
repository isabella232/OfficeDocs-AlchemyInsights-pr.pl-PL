---
title: Nowoczesna Strona jako Strona główna
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054712"
---
# <a name="modern-site-as-root-site"></a>Nowoczesna Strona jako Strona główna

Zaczęliśmy wdrożyć nową funkcję, która pozwoli Ci [zamienić swoją klasyczną stronę główną witryny z nowoczesną stroną](https://docs.microsoft.com/sharepoint/modern-root-site). Użyj [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) do zamiany lokalizacji witryny z innej witryny podczas archiwizacji oryginalnej witryny. Dostępne zarówno dla witryny zespołu (niepołączonej z grupą), jak i witryny komunikacyjnej.

>[!Important]
> Nie usuwaj klasycznej witryny głównej, aby utworzyć nowoczesną witrynę komunikacyjną. Nie jest to obsługiwane przez firmę Microsoft. Usunięcie witryny głównej spowoduje, że wszystkie witryny programu SharePoint w organizacji będą niedostępne dla wszystkich użytkowników, dopóki nie przywrócisz witryny lub nie utworzysz nowej witryny pod tym samym adresem URL. Będziemy komunikować tę funkcję za pośrednictwem centrum wiadomości. Należy się spodziewać funkcji, które mają być włączone w dzierżawie wkrótce.

## <a name="known-issues-with-swapping-sites"></a>Znane problemy z zamianę witryn
- Witryna docelowa może zwracać błąd "nie znaleziono" (HTTP 404) przez krótki okres czasu.
- Aby zaktualizować indeks wyszukiwania, konieczne będzie ponowne zaindeksowanie zawartości. Tu jest nie ręczny krok wymagany tutaj, ten mają być sporządzony mechanicznie.
- Wszystko, co jest zależne od "statyczne" łącza (takie jak pliki synchronizacji plików i OneNote) należy ręcznie skorygować.
- Witryny programu Project Server może wymagać sprawdzania poprawności, aby upewnić się, że są nadal skojarzone poprawnie. 

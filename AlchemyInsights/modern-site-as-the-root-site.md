---
title: Nowoczesne witryny jako witryny głównej
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620769"
---
# <a name="modern-site-as-root-site"></a>Nowoczesne witryny jako witryny głównej

Rozpoczęliśmy do rozmieszczenia nową funkcję, która pozwoli Ci o zamianę klasycznej strony głównej witrynie z nowoczesnymi witryny. Użyj [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Aby zamienić lokalizację witryny z innej witryny podczas archiwizowania oryginalnej witryny. Dostępne zarówno dla (nie połączeni z grupą) witryny zespołu i witryny komunikacji. 

>[!Important]
> Nie należy usuwać klasyczny głównej witrynie do tworzenia nowoczesnych witryny komunikacji. Nie jest to obsługiwane przez firmę Microsoft. Usunięcie katalogu głównego witryny spowoduje, że wszystkie witryny programu SharePoint w organizacji niedostępne dla wszystkich użytkowników, dopóki Przywracanie witryny lub utworzyć nową witrynę o takim samym adresie URL. Firma Microsoft będzie komunikować się tej funkcji za pośrednictwem Centrum wiadomości. Należy się spodziewać funkcji należy włączyć w dzierżawie wkrótce.

## <a name="known-issues-with-swapping-sites"></a>Znane problemy związane z zamiana stron
- Witryna docelowa może zwrócić "nie znaleziono" błąd (HTTP 404) krótki okres czasu.
- Zawartość będzie musiał być wykonane ponowne przeszukiwanie indeksu wyszukiwania. Nie procesu ręcznego tutaj, ten odbywa się automatycznie.
- Wszystko zależy od "static" łączy (na przykład pliki synchronizacji plików i program OneNote) będzie musiał ręcznie korygowana.
- Project Server witryn może muszą zostać zatwierdzone do zapewnienia, że są nadal skojarzona poprawnie. 

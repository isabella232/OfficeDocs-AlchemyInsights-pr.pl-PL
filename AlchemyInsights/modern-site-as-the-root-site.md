---
title: Nowoczesne witryny jako witryny głównej
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232725"
---
# <a name="modern-site-as-root-site"></a>Nowoczesne witryny jako witryny głównej

Rozpoczęliśmy do rozmieszczenia nową funkcję, która pozwoli Ci o zamianę klasycznej strony głównej witrynie z nowoczesnymi witryny. Użyj [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Aby zamienić lokalizację witryny z innej witryny podczas archiwizowania oryginalnej witryny. Dostępne zarówno dla (nie połączeni z grupą) witryny zespołu i witryny komunikacji. 

>[!Important]
> Nie należy usuwać klasyczny głównej witrynie do tworzenia nowoczesnych witryny komunikacji. Nie jest to obsługiwane przez firmę Microsoft. Usunięcie katalogu głównego witryny spowoduje, że wszystkie witryny programu SharePoint w organizacji niedostępne dla wszystkich użytkowników, dopóki Przywracanie witryny lub utworzyć nową witrynę o takim samym adresie URL. Firma Microsoft będzie komunikować się tej funkcji za pośrednictwem Centrum wiadomości. Należy się spodziewać funkcji należy włączyć w dzierżawie wkrótce.

## <a name="known-issues-with-swapping-sites"></a>Znane problemy związane z zamiana stron
- Witryna docelowa może zwrócić "nie znaleziono" błąd (HTTP 404) krótki okres czasu.
- Zawartość będzie musiał być wykonane ponowne przeszukiwanie indeksu wyszukiwania. Nie procesu ręcznego tutaj, ten odbywa się automatycznie.
- Wszystko zależy od "static" łączy (na przykład pliki synchronizacji plików i program OneNote) będzie musiał ręcznie korygowana.
- Project Server witryn może muszą zostać zatwierdzone do zapewnienia, że są nadal skojarzona poprawnie. 

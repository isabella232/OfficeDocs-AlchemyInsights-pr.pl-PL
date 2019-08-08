---
title: Zamień Classic głównej witrynie z nowoczesnymi witryny
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246041"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamień Classic głównej witrynie z nowoczesnymi witryny

Jeśli środowisku była skonfigurowana przed 2019 kwietnia, można zmienić głównej witrynie do nowoczesnego witryny za pomocą Microsoft PowerShell:

- Jeśli masz inną witrynę, którą chcesz używać jako głównej witrynie można zastąpić (wymiany) katalogu głównego witryny z nim. 
    - Użyj [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Aby zamienić lokalizację witryny z innej witryny podczas archiwizowania oryginalnej witryny. Dostępne zarówno dla (nie połączeni z grupą) witryny zespołu i witryny komunikacji. 

- Dodatkowe możliwości pojawią się wkrótce pozwoli Ci utrzymać korzystania z zawartości w witrynie, ale Konwertowanie istniejącej witryny do witryny komunikacji. 
>[!Important]
>Te możliwości będzie wdrażany stopniowo. Nadal sprawdzać Centrum Office 365 wiadomości dla aktualizacji. 

## <a name="known-issues-with-swapping-sites"></a>Znane problemy związane z zamiana stron

- Witryna docelowa może zwrócić "nie znaleziono" błąd (HTTP 404) krótki okres czasu.
- Zawartość będzie musiał być wykonane ponowne przeszukiwanie indeksu wyszukiwania. Nie procesu ręcznego wymagane - ten odbywa się automatycznie.
- Wszystko zależy od "static" łączy (na przykład pliki synchronizacji plików i program OneNote) będzie musiał ręcznie korygowana.
- Jeśli źródłowa witryna witryny wiadomości dotyczące organizacji, należy zaktualizować adres URL.Wyświetlić listę wszystkich witryn wiadomości dotyczące organizacji.
- Project Server witryn może muszą zostać zatwierdzone do zapewnienia, że są nadal skojarzona poprawnie.






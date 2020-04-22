---
title: Zawartość nie jest wyświetlana w wynikach wyszukiwania programu SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705671"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Zawartość nie jest wyświetlana w wynikach wyszukiwania programu SharePoint

Wykonaj następujące kroki rozwiązywania problemów, gdy oczekiwana zawartość nie jest wyświetlana w wynikach wyszukiwania:
  
1. Sprawdź, czy **witryna** zawierająca oczekiwaną zawartość jest ustawiona tak, aby zawartość wyświetlała się w wynikach wyszukiwania. Wykonaj czynności opisane w obszarze [Pokazywalaj zawartość w witrynie w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Sprawdź, czy **lista** lub **biblioteka zawierająca** oczekiwaną zawartość jest ustawiona tak, aby zawartość wyświetlała się w wynikach wyszukiwania. Wykonaj czynności opisane w obszarze [Pokazywalaj zawartość z list lub bibliotek w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Sprawdź, czy układ strony, dokumentu lub strony niestandardowej jest publikowany jako **wersja główna.** Wykonaj krok 3 w [wyszukiwarce nie zwraca wszystkich wyników w usłudze SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Sprawdź, czy użytkownik ma **uprawnienia** do wyświetlania zawartości. Wykonaj kroki opisane w [opisie poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Jeśli schemat wyszukiwania został zmieniony przez dodanie nowej właściwości zarządzanej, przez edycję właściwości zarządzanej lub przez usunięcie właściwości zarządzanej, wymagane będzie żądanie indeksowania i ponownego indeksowania. **Ponownie indeksuj** zawartość, wykonując czynności opisane w [Ręcznym żądaniu indeksowania i ponownego indeksowania witryny, biblioteki lub listy](https://docs.microsoft.com/sharepoint/crawl-site-content). Może to trochę potrwać, odczekaj 24 godziny przed ponownym sprawdzeniem wyników.

Aby uzyskać więcej informacji, zobacz [Włączanie przeszukiwania zawartości witryny](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  

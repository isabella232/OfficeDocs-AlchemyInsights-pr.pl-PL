---
title: Zawartość nie jest wyświetlana w SharePoint wyszukiwania
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081620"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Zawartość nie jest wyświetlana w SharePoint wyszukiwania

Wykonaj poniższe czynności rozwiązywania problemów, gdy oczekiwana zawartość nie pojawia się w wynikach wyszukiwania:
  
1. Upewnij się, **że witryna zawierająca** oczekiwaną zawartość jest ustawiona tak, aby zezwalała na jej pojawianie się w wynikach wyszukiwania. Postępuj zgodnie z instrukcjami [w tece Pokazywanie zawartości witryny w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Upewnij się, **że na liście** lub **w** bibliotece zawierającej oczekiwaną zawartość jest ustawiona zezwalanie na pojawianie się zawartości w wynikach wyszukiwania. Postępuj zgodnie z instrukcjami [w artykule Pokazywanie zawartości z list lub bibliotek w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Sprawdź, czy strona, dokument lub niestandardowy układ strony jest opublikowana jako **wersja główna.** Wykonaj krok 3 w funkcji wyszukiwania nie zwraca wszystkich wyników w u [SharePoint Online.](https://go.microsoft.com/fwlink/?linkid=874525)

4. Sprawdź, czy użytkownik ma **uprawnienia do** wyświetlania zawartości. Wykonaj czynności opisane w [opisie poziomów uprawnień w programie SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
    
5. Jeśli schemat wyszukiwania został zmieniony przez dodanie nowej właściwości zarządzanej, edytowanie właściwości zarządzanej lub przez usunięcie właściwości zarządzanej, będzie wymagane żądanie przeszukiwania i ponownego indeksowania. **Ponownie zaindeksuj** zawartość, korzystając z procedury opisanej w te sposób: Ręczne żądanie przeszukiwania i ponownego indeksowania witryny, biblioteki [lub listy.](https://docs.microsoft.com/sharepoint/crawl-site-content) Może to trochę potrwać, odczekaj 24 godziny, zanim ponownie sprawdzisz wyniki.

Aby uzyskać więcej informacji, zobacz Włączanie przeszukiwania zawartości [witryny.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  

---
title: Zawartość nie jest wyświetlana w wynikach wyszukiwania w programie SharePoint
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
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713140"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Zawartość nie jest wyświetlana w wynikach wyszukiwania w programie SharePoint

Wykonaj te czynności rozwiązywania problemów, gdy oczekiwana zawartość nie zostanie wyświetlona w wynikach wyszukiwania:
  
1. Sprawdź, czy **Witryna** zawierająca oczekiwaną zawartość jest ustawiona tak, aby zezwalać na wyświetlanie zawartości w wynikach wyszukiwania. Wykonaj czynności podane w artykule [Pokazywanie zawartości witryny w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Sprawdź, czy **Lista** lub **Biblioteka** zawierająca oczekiwaną zawartość jest ustawiona tak, aby zezwalać na wyświetlanie zawartości w wynikach wyszukiwania. Postępuj zgodnie z instrukcjami podanymi w [artykule pokazywanie zawartości z list lub bibliotek w wynikach wyszukiwania](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Sprawdź, czy strona, dokument lub niestandardowy układ strony jest opublikowany jako **wersja główna.** Obserwuj krok 3 w funkcji [wyszukiwania nie są zwracane wszystkie wyniki w usłudze SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Sprawdź, czy użytkownik ma **uprawnienia** do wyświetlania zawartości. Postępuj zgodnie z instrukcjami podanymi w artykule [Omówienie poziomów uprawnień w programie SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Jeśli schemat wyszukiwania został zmieniony przez dodanie nowej właściwości zarządzanej, edytując właściwość zarządzaną lub usuwając właściwość zarządzaną, wymagane jest ponowne przeszukiwanie i ponowne indeksowanie. **Ponownie Indeksuj** zawartość, wykonując czynności opisane w temacie [Ręczne żądanie przeszukiwania i ponowne indeksowanie witryny, biblioteki lub listy](https://docs.microsoft.com/sharepoint/crawl-site-content). Może to trochę potrwać, odczekaj 24 godziny, zanim ponownie sprawdzisz wyniki.

Aby uzyskać więcej informacji, zobacz [Włączanie funkcji wyszukiwania zawartości w witrynie](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  

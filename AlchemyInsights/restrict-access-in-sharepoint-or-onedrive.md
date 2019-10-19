---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551461"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w programie SharePoint lub OneDrive

W programie SharePoint i usłudze OneDrive można ograniczyć dostęp do elementów, takich jak pliki, foldery i listy, udzielając dostępu tylko grupom lub osobom, które mają mieć dostęp. Domyślnie uprawnienia w programie SharePoint są dziedziczone z wyższych w hierarchii. Więc plik dziedziczy uprawnienia z folderu, który dziedziczy jego uprawnienia z biblioteki, która dziedziczy jej uprawnienia z witryny.
  
Można udostępnić na wyższym poziomie (na przykład przez udostępnianie całej witryny), a następnie przerwać dziedziczenie, jeśli nie chcesz udostępniać wszystkie elementy w witrynie. Jednak nie zaleca się tego, ponieważ sprawia, że utrzymanie uprawnień bardziej skomplikowane i mylące w przyszłości. Oto, co można zrobić zamiast:
  
- Jeśli na przykład chcesz udostępnić całą zawartość folderu z wyjątkiem jednego pliku, Przenieś ten plik do nowej lokalizacji, która nie jest udostępniana.
    
- Jeśli masz dwa podfoldery w folderze i chcesz udostępnić jeden podfolder grupom A i B i zezwolić tylko na dostęp do drugiego podfolderu, Udostępnij folder nadrzędny grupie A i Dodaj grupę B do pierwszego podfolderu.
    
[Zatrzymywanie udostępniania pliku lub folderu](https://go.microsoft.com/fwlink/?linkid=2008861)
  


---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28304647"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w programie SharePoint lub OneDrive

W programie SharePoint i OneDrive możesz ograniczyć dostęp do elementów, takich jak pliki, foldery i list poprzez przyznanie dostępu tylko do grup lub osób, które chcesz mieć dostęp. Domyślnie uprawnienia w programie SharePoint są dziedziczone z wyżej w hierarchii. Tak więc plik dziedziczą uprawnienia z folderu, który dziedziczy uprawnienia z biblioteki, która dziedziczy uprawnienia z witryny.
  
Można udostępniać na wyższym poziomie (takich jak Udostępnianie całej witryny) i następnie przerwać dziedziczenie, jeśli nie chcesz udostępniać wszystkie elementy na stronie. Jednak nie jest to zalecane, ponieważ to sprawia, że utrzymywanie uprawnienia bardziej skomplikowana i myląca w przyszłości. Oto, co można zrobić w zamian:
  
- Jeśli na przykład chcesz udostępnić całą zawartość folderu z wyjątkiem jednego pliku w nim, należy przenieść ten plik do nowej lokalizacji, która nie jest udostępniony.
    
- Jeśli masz dwa podfoldery w folderze, a chcesz udostępnić jeden podfolder z grupy A i B oraz dostęp do tylko grupa A drugi podfolderu, udostępnić folder nadrzędny z grupy A i dodać grupy B do pierwszego podfolderu.
    
[Zatrzymaj udostępnianie pliku lub folderu](https://go.microsoft.com/fwlink/?linkid=2008861)
  


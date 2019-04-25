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
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383881"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w programie SharePoint lub OneDrive

W programie SharePoint i OneDrive możesz ograniczyć dostęp do elementów, takich jak pliki, foldery i list poprzez przyznanie dostępu tylko do grup lub osób, które chcesz mieć dostęp. Domyślnie uprawnienia w programie SharePoint są dziedziczone z wyżej w hierarchii. Tak więc plik dziedziczą uprawnienia z folderu, który dziedziczy uprawnienia z biblioteki, która dziedziczy uprawnienia z witryny.
  
Można udostępniać na wyższym poziomie (takich jak Udostępnianie całej witryny) i następnie przerwać dziedziczenie, jeśli nie chcesz udostępniać wszystkie elementy na stronie. Jednak nie jest to zalecane, ponieważ to sprawia, że utrzymywanie uprawnienia bardziej skomplikowana i myląca w przyszłości. Oto, co można zrobić w zamian:
  
- Jeśli na przykład chcesz udostępnić całą zawartość folderu z wyjątkiem jednego pliku w nim, należy przenieść ten plik do nowej lokalizacji, która nie jest udostępniony.
    
- Jeśli masz dwa podfoldery w folderze, a chcesz udostępnić jeden podfolder z grupy A i B oraz dostęp do tylko grupa A drugi podfolderu, udostępnić folder nadrzędny z grupy A i dodać grupy B do pierwszego podfolderu.
    
[Zatrzymaj udostępnianie pliku lub folderu](https://go.microsoft.com/fwlink/?linkid=2008861)
  


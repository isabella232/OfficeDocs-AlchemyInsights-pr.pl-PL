---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715894"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w programie SharePoint lub OneDrive

W programie SharePoint i OneDrive ograniczasz dostęp do elementów, takich jak pliki, foldery i listy, przyznając dostęp tylko grupom lub osobom, do których chcesz mieć dostęp. Domyślnie uprawnienia w programie SharePoint są dziedziczone z wyższej pozycji w hierarchii. Tak więc plik dziedziczy jego uprawnienia z folderu, który dziedziczy jego uprawnienia z biblioteki, która dziedziczy jego uprawnienia z witryny.
  
Możesz udostępniać na wyższym poziomie (na przykład udostępniając całą witrynę), a następnie przerywać dziedziczenie, jeśli nie chcesz udostępniać wszystkich elementów w witrynie. Jednak nie zaleca się tego, ponieważ sprawia, że utrzymanie uprawnień bardziej skomplikowane i mylące w przyszłości. Oto, co możesz zrobić:
  
- Jeśli na przykład chcesz udostępnić całą zawartość folderu z wyjątkiem jednego pliku, przenieś ten plik do nowej lokalizacji, która nie jest udostępniana.
    
- Jeśli w folderze są dwa podfoldery, a jeden podfolder chcesz udostępnić jeden podfolder grupom A i B oraz zezwolić tylko grupie A na dostęp do drugiego podfolderu, udostępnij folder nadrzędny grupie A i dodaj grupę B do pierwszego podfolderu.
    
[Zatrzymywanie udostępniania pliku lub folderu](https://go.microsoft.com/fwlink/?linkid=2008861)
  


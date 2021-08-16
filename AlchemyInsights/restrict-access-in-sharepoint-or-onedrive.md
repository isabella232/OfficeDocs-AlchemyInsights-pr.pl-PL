---
title: Ograniczanie dostępu w SharePoint lub OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075050"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w SharePoint lub OneDrive

W SharePoint i OneDrive dostęp do elementów, takich jak pliki, foldery i listy, można ograniczyć, udzielając dostępu tylko grupom lub osobom, które mają mieć dostęp. Domyślnie uprawnienia w większej SharePoint są dziedziczone z wyższego poziomu hierarchii. Dlatego plik dziedziczy swoje uprawnienia po folderze, który dziedziczy swoje uprawnienia po bibliotece, która dziedziczy uprawnienia po witrynie.
  
Jeśli nie chcesz udostępniać wszystkich elementów w witrynie, możesz udostępnić ją na wyższym poziomie (na przykład przez udostępnienie całej witryny), a następnie przerwać dziedziczenie. Nie jest to jednak zalecane, ponieważ powoduje to, że utrzymywanie uprawnień jest bardziej złożone i mylące w przyszłości. Zamiast tego możesz wykonać te dzieje się tak:
  
- Jeśli na przykład chcesz udostępnić całą zawartość folderu z wyjątkiem jednego pliku w tym folderze, przenieś ten plik do nowej lokalizacji, która nie jest udostępniana.
    
- Jeśli masz w folderze dwa podfoldery i chcesz udostępnić jeden podfolder grupom A i B i zezwolić tylko grupie A na dostęp do drugiego podfolderu, udostępnij folder nadrzędny grupie A i dodaj grupę B do pierwszego podfolderu.
    
[Zatrzymywanie udostępniania pliku lub folderu ](https://go.microsoft.com/fwlink/?linkid=2008861)
  


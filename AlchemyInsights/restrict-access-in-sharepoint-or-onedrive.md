---
title: Ograniczanie dostępu w programie SharePoint lub usłudze OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720692"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograniczanie dostępu w programie SharePoint lub usłudze OneDrive

W programie SharePoint i usłudze OneDrive możesz ograniczyć dostęp do elementów, takich jak pliki, foldery i listy, udzielając dostępu tylko grupom lub osobom, do których chcesz mieć dostęp. Domyślnie uprawnienia w programie SharePoint są dziedziczone z wyższego poziomu w hierarchii. Dzięki temu plik dziedziczy uprawnienia z folderu, który dziedziczy uprawnienia z biblioteki, co powoduje dziedziczenie uprawnień do witryny.
  
Możesz udostępnić na wyższym poziomie (na przykład udostępnić całą witrynę), a następnie przerwać dziedziczenie, jeśli nie chcesz udostępniać wszystkich elementów w witrynie. Nie jest to jednak zalecane, ponieważ ułatwia to zachowanie uprawnień bardziej złożonych i mylących w przyszłości. Możesz to zrobić w następujący sposób:
  
- Jeśli na przykład chcesz udostępnić całą zawartość folderu z wyjątkiem jednego pliku, Przenieś ten plik do nowej lokalizacji, która nie jest udostępniona.
    
- Jeśli w folderze znajdują się dwa podfoldery i chcesz udostępnić pojedynczy podfolder grupom a i B i zezwolić tylko na grupowanie w drugim podfolderze, Udostępnij folder nadrzędny grupie A i Dodaj grupę B do pierwszego podfolderu.
    
[Zatrzymywanie udostępniania pliku lub folderu ](https://go.microsoft.com/fwlink/?linkid=2008861)
  


---
title: Przepływ pracy nie jest rozpoczynany
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049347"
---
# <a name="workflow-is-not-starting"></a>Przepływ pracy nie jest rozpoczynany

- Nie są uruchamianie przepływów pracy programu SharePoint 2010 i SharePoint 2013.

    - Jeśli przepływ pracy nie jest uruchamianie, może być problem tymczasowy usługi, gdzie użytkownicy mogą wystąpić sporadyczne opóźnienia z postępu przepływu pracy. Sprawdź [pulpit nawigacyjny kondycji usługi](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , aby sprawdzić, czy Twoja organizacja ma wpływ.

    - Jeśli minęło więcej niż 24 godziny od pierwszego zobaczyłem ten problem, należy zalogować bilet pomocy technicznej. W wielu przypadkach pracujemy już nad rozwiązaniem. Proszę dać nam co najmniej 24 godziny, aby zakończyć rozwiązanie.

- Przepływy pracy programu SharePoint 2010 opóźnione podczas uruchamiania.

    - Dzieje się tak, jeśli przepływ pracy jest wyzwalany w dużych partiach. (na przykład, gdy kilka elementów są dodawane jednocześnie).

    - Przepływy pracy nie są przeznaczone do uruchamiania w czasie rzeczywistym, więc opóźnienie jest zachowanie przez projekt.

   -  Jeśli przepływ pracy jest złożony Extensible Object Markup Language (XMOL), kompilacja może być powolne. Sprawdź [ten](https://support.microsoft.com//kb/3043697) artykuł.

    - Należy uprościć przepływ pracy lub przeprojektować go przy użyciu typu platformy Microsoft SharePoint 2013 przepływu pracy.

    - Jeśli Historia przepływu pracy wzrosła, możesz chcieć usunąć elementy lub utworzyć nową listę historii.

        Więcej informacji: [Wyczyść historię przepływu pracy](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tematy pokrewne
Chcesz wypróbować usługi Microsoft Flow w usłudze SharePoint Online?
- [Utwórz przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i przepływu](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



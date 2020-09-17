---
title: Przepływ pracy nie jest uruchamiany
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794777"
---
# <a name="workflow-is-not-starting"></a>Przepływ pracy nie jest uruchamiany

- Nie można uruchomić przepływów pracy programu SharePoint 2010 i SharePoint 2013.

    - Jeśli przepływ pracy nie rozpoczyna się, może to oznaczać, że wystąpił tymczasowy problem z usługą, w którym użytkownicy mogą napotykać sporadycznie opóźnienia z postępem przepływu pracy. Sprawdź [pulpit nawigacyjny kondycji usługi](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , aby sprawdzić, czy Twoja organizacja ma wpływ na.

    - Jeśli od momentu pierwszego uruchomienia tego problemu minęło więcej niż 24 godziny, zarejestruj bilet pomocy technicznej. W wielu przypadkach jesteśmy już nad rozwiązaniem. Przekaż nam co najmniej 24 godziny na zakończenie rozwiązania.

- Przepływy pracy programu SharePoint 2010 opóźnione od uruchomienia.

    - Dzieje się tak, jeśli przepływ pracy zostanie wyzwolony w dużych partiach. (na przykład po dodaniu kilku elementów jednocześnie).

    - Przepływy pracy nie są przeznaczone do uruchamiania w czasie rzeczywistym, więc zachowanie polega na zaprojektowaniu.

   -  Jeśli przepływ pracy jest skomplikowanym językiem Extensible Object Markup Language (XMOL), kompilacja może potrwać wolno. Sprawdź [ten](https://support.microsoft.com//kb/3043697) artykuł.

    - W celu uproszczenia przepływu pracy lub zaprojektowania go możesz go ponownie użyć na platformie przepływu pracy programu Microsoft SharePoint 2013.

    - Jeśli Historia przepływu pracy jest duża, możesz chcieć przeczyścić te elementy lub utworzyć nową listę historii.

        Więcej informacji: [przeczyszczanie historii przepływu pracy](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tematy pokrewne
Chcesz wypróbować przepływ pracy Microsoft w usłudze SharePoint Online?
- [Utwórz przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Program SharePoint i przepływ](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



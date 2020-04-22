---
title: Przepływ pracy nie jest uruchamiany
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766107"
---
# <a name="workflow-is-not-starting"></a>Przepływ pracy nie jest uruchamiany

- Nie uruchamiają się przepływów pracy programu SharePoint 2010 i SharePoint 2013.

    - Jeśli przepływ pracy nie jest uruchamiany, może to być tymczasowy problem z usługą, w którym użytkownicy mogą doświadczać sporadyczne opóźnienia z postępem przepływu pracy. Sprawdź pulpit nawigacyjny [kondycji usługi,](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) aby sprawdzić, czy twoja organizacja ma wpływ.

    - Jeśli od pierwszego zobaczenia tego problemu minęło więcej niż 24 godziny, zarejestruj bilet pomocy technicznej. W wielu przypadkach już pracujemy nad rozwiązaniem. Daj nam co najmniej 24 godziny na uzupełnienie rozwiązania.

- Przepływy pracy programu SharePoint 2010 opóźnione przy uruchomieniu.

    - Dzieje się tak, jeśli przepływ pracy jest wyzwalany w dużych partiach. (na przykład, gdy kilka elementów są dodawane naraz).

    - Przepływy pracy nie są przeznaczone do uruchamiania w czasie rzeczywistym, więc opóźnienie jest zachowaniem według projektu.

   -  Jeśli przepływ pracy jest złożony extensible Object Markup Language (XMOL), kompilacja może być powolna. Sprawdź [ten](https://support.microsoft.com//kb/3043697) artykuł.

    - Należy uprościć przepływ pracy lub przeprojektować go przy użyciu typu platformy przepływów pracy programu Microsoft SharePoint 2013.

    - Jeśli historia przepływu pracy stała się duża, można przeczyścić elementy lub utworzyć nową listę historii.

        Więcej informacji : [Historia przepływu pracy przeczyszczanie](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tematy pokrewne
Chcesz wypróbować usługę Microsoft Flow w usłudze SharePoint Online?
- [Utwórz przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Program SharePoint i przepływ](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



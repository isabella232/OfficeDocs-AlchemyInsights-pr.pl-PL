---
title: Przepływ pracy nie jest rozpoczynany
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403753"
---
# <a name="workflow-is-not-starting"></a>Przepływ pracy nie jest rozpoczynany

- Przepływy pracy programu SharePoint 2010 i SharePoint 2013 nie są rozpoczynane.

    - Jeśli przepływ pracy nie jest rozpoczynany, może wystąpić tymczasowy problem z usługą, w przypadku którego użytkownicy mogą mieć sporadyczne opóźnienia z postępem przepływu pracy. Sprawdź na [pulpicie nawigacyjnym kondycji](https://admin.microsoft.com/AdminPortal/Home/servicehealth) usług, czy wpływa to na Twoją organizację.

    - Jeśli od pierwszego problemu minęły ponad 24 godziny, zaloguj bilet pomocy technicznej. W wielu przypadkach pracujemy już nad rozwiązaniem. Daj nam co najmniej 24 godziny, aby ukończyć rozwiązanie.

- Przepływy pracy programu SharePoint 2010 opóźnione po uruchomieniu.

    - Dzieje się tak, jeśli przepływ pracy jest wyzwalany w dużych partiach. (na przykład gdy kilka elementów jest dodawanych jednocześnie).

    - Przepływy pracy nie są zaprojektowane do uruchamiania w czasie rzeczywistym, więc opóźnienie jest procesem projektu.

   -  Jeśli przepływ pracy jest złożonym językiem X JIM (Extensible Object Markup Language), kompilacja może być spowalniana. Zapoznaj się [z tym](https://support.microsoft.com//kb/3043697) artykułem.

    - Należy uprościć przepływ pracy lub przeprojektować go przy użyciu typu platformy przepływów pracy programu Microsoft SharePoint 2013.

    - Jeśli Twoja historia przepływu pracy się powiększy, możesz usunąć elementy lub utworzyć nową listę historii.

        Więcej informacji: [Przeczyszczanie historii przepływu pracy](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tematy pokrewne
Chcesz wypróbować usługę Microsoft Flow w usłudze SharePoint Online?
- [Tworzenie przepływu](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 

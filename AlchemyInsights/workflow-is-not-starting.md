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
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907748"
---
# <a name="workflow-is-not-starting"></a>Przepływ pracy nie jest rozpoczynany

- SharePoint 2010 i SharePoint 2013 nie są rozpoczynane.

    - Jeśli przepływ pracy nie jest rozpoczynany, może wystąpić tymczasowy problem z usługą, w przypadku którego użytkownicy mogą mieć sporadyczne opóźnienia z postępem przepływu pracy. Sprawdź na [pulpicie nawigacyjnym kondycji](https://admin.microsoft.com/AdminPortal/Home/servicehealth) usług, czy wpływa to na Twoją organizację.

    - Jeśli od pierwszego problemu minęły ponad 24 godziny, zaloguj bilet pomocy technicznej. W wielu przypadkach pracujemy już nad rozwiązaniem. Daj nam co najmniej 24 godziny, aby ukończyć rozwiązanie.

- SharePoint 2010 przepływów pracy opóźnionych podczas uruchamiania.

    - Dzieje się tak, jeśli przepływ pracy jest wyzwalany w dużych partiach. (na przykład gdy kilka elementów jest dodawanych jednocześnie).

    - Przepływy pracy nie są zaprojektowane do uruchamiania w czasie rzeczywistym, więc opóźnienie jest procesem projektu.

   -  Jeśli przepływ pracy jest złożonym językiem X JIM (Extensible Object Markup Language), kompilacja może być spowalniana. Zapoznaj się [z tym](https://support.microsoft.com//kb/3043697) artykułem.

    - Należy uprościć przepływ pracy lub przeprojektować go przy użyciu typu platformy przepływów SharePoint Microsoft SharePoint 2013.

    - Jeśli Twoja historia przepływu pracy się powiększy, możesz usunąć elementy lub utworzyć nową listę historii.

        Więcej informacji: [Przeczyszczanie historii przepływu pracy](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Tematy pokrewne
Chcesz wypróbować te Microsoft Flow w SharePoint Online?
- [Tworzenie Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 

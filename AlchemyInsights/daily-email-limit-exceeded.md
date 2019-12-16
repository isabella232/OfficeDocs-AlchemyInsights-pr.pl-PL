---
title: Przekroczono dzienny limit wiadomości e-mail. Przepływ pracy jest zawieszony.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053127"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Przekroczono limit dziennego limitu e-mail. Przepływ pracy jest zawieszony.

Ten błąd może zostać odebrany w następujących scenariuszach:

- Masz przepływu pracy w programie SharePoint w trybie online, który używa programu SharePoint 2010 lub SharePoint 2013 typ platformy przepływu pracy.
- Przepływ pracy jest skonfigurowany do wysyłania niestandardowej wiadomości e-mail do więcej niż 200 użytkowników w czasie, więcej niż 10 000 adresatów dziennie lub więcej niż 30 wiadomości na minutę.
- Po uruchomieniu przepływu pracy, wiadomość e-mail nie jest wysyłana i można zauważyć następujące zachowanie:
    - Dla przepływu pracy przy użyciu typu platformy SharePoint 2013, przejdź do strony **stan przepływu pracy** . Na stronie stan przepływu pracy **stan wewnętrzny** jest ustawiony na wartość **rozpoczęte**, a w dymku informacyjnym **nie można wysyłać do adresata**.

Aby obejść ten problem, skonfiguruj przepływ pracy do wysyłania wiadomości e-mail bez przekraczania [limitów nadawcy programu Exchange w trybie online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na przykład należy użyć pauzy w przepływie pracy, wysłać wiadomość e-mail do grupy 365 pakietu Office, grupy dystrybucyjnej lub grupy zabezpieczeń z włączoną obsługą poczty lub wysłać ją do mniej niż 200 adresatów naraz.


Aby uzyskać więcej informacji, zobacz następujący [artykuł](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Tematy pokrewne
- [Utwórz przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i przepływu](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
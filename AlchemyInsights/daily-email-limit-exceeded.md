---
title: Przekroczono dzienny limit poczty e-mail. Przepływ pracy jest wstrzymany.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731573"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Przekroczono dzienny limit poczty e-mail. Przepływ pracy jest wstrzymany.

Ten błąd może zostać odebrany w następujących scenariuszach:

- Masz przepływ pracy w usłudze SharePoint Online, w którym jest używany typ platformy przepływ pracy programu SharePoint 2010 lub SharePoint 2013.
- W ramach przepływu pracy skonfigurowano wysyłanie niestandardowej wiadomości e-mail do ponad 200 użytkowników jednocześnie, ponad 10 000 adresatów dziennie lub więcej niż 30 wiadomości na minutę.
- Po uruchomieniu przepływu pracy wiadomość e-mail nie jest wysyłana, a Użytkownik zauważy następujące zachowanie:
    - W przypadku przepływu pracy korzystającego z typu platformy programu SharePoint 2013 przejdź do strony **stan przepływu pracy** . Na stronie stan przepływu pracy jest ustawiany **stan wewnętrzny** **, a**w dymku informacji jest wyświetlany komunikat **nie można wysłać do adresata**.

Aby obejść ten problem, skonfiguruj przepływ pracy w celu wysyłania wiadomości e-mail bez przekroczenia [limitów nadawcy usługi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na przykład w przepływie pracy można użyć funkcji wstrzymania, wysłać wiadomość e-mail 365 do grupy dystrybucyjnej, grupy dystrybucyjnej lub grupy zabezpieczeń z obsługą poczty albo wysłać wiadomość do mniej niż 200 adresatów jednocześnie.


Aby uzyskać więcej informacji, zobacz następujący [artykuł](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Tematy pokrewne
- [Utwórz przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Program SharePoint i przepływ](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
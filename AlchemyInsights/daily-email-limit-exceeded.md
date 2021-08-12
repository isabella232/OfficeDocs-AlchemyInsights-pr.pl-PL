---
title: Przekroczono dzienny limit poczty e-mail. Przepływ pracy zostanie zawieszony.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914661"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Przekroczono dzienny limit poczty e-mail. Przepływ pracy zostanie zawieszony.

Ten błąd może zostać odebrany w następujących scenariuszach:

- Masz przepływ pracy w aplikacji SharePoint Online, który używa typu platformy przepływów SharePoint 2010 SharePoint 2013.
- Przepływ pracy jest skonfigurowany do wysyłania niestandardowej wiadomości e-mail do ponad 200 użytkowników jednocześnie, do ponad 10 000 adresatów dziennie lub do ponad 30 wiadomości na minutę.
- Po uruchomieniu przepływu pracy wiadomość e-mail nie zostanie wysłana i zauważysz następujące zachowanie:
    - W przypadku przepływu pracy korzystającego SharePoint typu platformy 2013 przejdź do strony **Stan przepływu** pracy. Na stronie Stan przepływu pracy dla pozycji **Stan** wewnętrzny ustawiono wartość Uruchomiliśmy, a w dymku informacji jest wyświetlany komunikat Nie można **wysłać do adresata.**

Aby ominą ten problem, skonfiguruj przepływ pracy w celu wysyłania wiadomości e-mail bez przekroczenia limitów Exchange Online [nadawców.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Możesz na przykład zatrzymać przepływ pracy, wysłać wiadomość e-mail do grupy programu Microsoft 365, grupy dystrybucyjnej lub grupy zabezpieczeń z obsługą poczty albo wysłać wiadomość do mniej niż 200 adresatów jednocześnie.


Aby uzyskać więcej informacji, zobacz następujący [artykuł.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Tematy pokrewne
- [Tworzenie Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
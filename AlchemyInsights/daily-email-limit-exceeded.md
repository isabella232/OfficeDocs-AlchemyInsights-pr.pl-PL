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
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580343"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dzienny limit wiadomości e-mail przekroczony. Przepływ pracy jest zawieszony.

Ten błąd może zostać odebrany w następujących scenariuszach:

- Przepływ pracy w usłudze SharePoint Online jest używany w typie platformy przepływu pracy programu SharePoint 2010 lub SharePoint 2013.
- Przepływ pracy jest skonfigurowany do wysyłania niestandardowej wiadomości e-mail do ponad 200 użytkowników naraz, ponad 10 000 adresatów dziennie lub więcej niż 30 wiadomości na minutę.
- Po uruchomieniu przepływu pracy wiadomość e-mail nie jest wysyłana i zauważysz następujące zachowanie:
    - W przypadku przepływu pracy przy użyciu typu platformy programu SharePoint 2013 można przejść do strony **Stan przepływu pracy.** Na stronie Stan przepływu pracy **stan wewnętrzny** jest ustawiony na **Uruchomiono,** a dymek informacji nie **może wysłać do adresata**.

Aby obejść ten problem, skonfiguruj przepływ pracy tak, aby wysyłał wiadomości e-mail bez [przekraczania limitów nadawców usługi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na przykład użyj pauzy w przepływie pracy, wyślij wiadomość e-mail do grupy microsoft 365, grupy dystrybucyjnej lub grupy zabezpieczeń z włączoną pocztą lub wyślij wiadomość do mniej niż 200 adresatów naraz.


Aby uzyskać więcej informacji, zobacz następujący [artykuł](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Tematy pokrewne
- [Utwórz przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Program SharePoint i przepływ](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
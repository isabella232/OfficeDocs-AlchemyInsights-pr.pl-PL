---
title: Przekroczono dzienny limit wiadomości e-mail. Przepływ pracy jest zawieszone.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514475"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Przekroczony Limit dzienny poczta elektroniczna. Przepływ pracy jest zawieszone.

Tego błędu mogą pojawić się w następujących scenariuszach:

- Masz przepływu pracy programu SharePoint Online używanego programu SharePoint 2010 lub typ platformy przepływu pracy programu SharePoint 2013.
- Przepływ pracy jest skonfigurowany do wysyłania wiadomości e-mail niestandardowych do więcej niż 200 użytkowników w czasie, więcej niż 10 000 adresatów dziennie lub więcej niż 30 wiadomości na minutę.
- Po uruchomieniu przepływu pracy nie jest wysyłana wiadomość e-mail, a można zauważyć następujące zachowanie:
    - Dla przepływu pracy przy użyciu typu platformy SharePoint 2013 przejdź do strony **Stan przepływu pracy** . Na stronie Stan przepływu pracy **Wewnętrzny stan** jest ustawiony na **Rozpoczęte**i wyświetla dymek informacyjny **nie można wysłać do adresata**.

Aby obejść ten problem, należy skonfigurować przepływu pracy do wysyłania wiadomości e-mail bez przekroczenia [limitów nadawcy programu Exchange w trybie Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na przykład za pomocą pause w przepływie pracy, Wyślij wiadomość e-mail do grupy usługi Office 365, grupy dystrybucyjnej lub grupy zabezpieczeń włączoną obsługę poczty lub wysłać wiadomość do mniej niż 200 adresatów naraz.


Aby uzyskać więcej informacji zobacz następujący [artykuł](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Tematy pokrewne
- [Utworzyć przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i przepływu](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
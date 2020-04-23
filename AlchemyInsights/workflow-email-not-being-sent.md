---
title: Nie jest wysyłana wiadomość e-mail z przepływem pracy
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
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766143"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Poczta e-mail przepływu pracy nie jest wysyłana dla listy lub biblioteki programu SharePoint

1. Wiadomości e-mail z przepływów pracy nie są wysyłane do wszystkich użytkowników lub tylko do określonych użytkowników lub pojawia się błąd **Nie można wysłać wiadomości e-mail. Upewnij się, że wiadomość e-mail ma prawidłowego adresata**.

    Sprawdź, czy użytkownik istnieje w grupie Uprawnienia **Wszystkie osoby** (lista informacji o użytkowniku) dla tego zbioru witryn.  Przykładowy bezpośredni adres URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? Udział w członkostwie=0

    - Jeśli użytkownik nie istnieje, upewnij się, że użytkownik jest zalogowany do strony. 
    - Jeśli jest to użytkownik zewnętrzny, upewnij się, że jego zaproszenie zostało zaakceptowane.
    - Jeśli użytkownik istnieje w grupie uprawnień, upewnij się, że adres e-mail jest poprawny.
    - Jeśli adres e-mail użytkowników nie jest w tym miejscu ustawiony, utwórz przykładowy alert dla tego użytkownika, który wymusza synchronizację tego konta użytkownika z profili użytkowników programu SharePoint do tego zbioru witryn.
 
2. Wiadomości e-mail z przepływów pracy są wysyłane do administratorów zbioru witryn, ale nie do innych użytkowników i zobacz błąd **HTTP zabronione <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Zobacz [Odmowa dostępu podczas wysyłania wiadomości e-mail do grupy programu SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Sprawdź również, czy funkcja zbierania witryn **w trybie blokady uprawnień użytkownika o ograniczonym dostępie** nie jest aktywna.


## <a name="related-topics"></a>Tematy pokrewne
Chcesz wypróbować usługę Microsoft Flow w usłudze SharePoint Online?
- [Utwórz przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Program SharePoint i przepływ](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



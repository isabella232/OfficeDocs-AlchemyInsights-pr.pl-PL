---
title: Nie jest wysyłany e-mail przepływu pracy
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
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530894"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mail przepływu pracy nie jest wysyłany do listy programu SharePoint lub biblioteki

1. Wiadomości e-mail z przepływów pracy nie są wysyłane do wszystkich użytkowników lub tylko określonych użytkowników lub widać, że błąd **wiadomość e-mail nie może zostać wysłana. Upewnić się, czy wiadomość e-mail ma prawidłowego adresata**.

    Sprawdź, czy użytkownik istnieje w grupie uprawnienia **Wszystkich osób** (Lista informacji o użytkownikach) dla tego zbioru witryn.  Przykładowe bezpośredni adres URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Jeśli użytkownik nie istnieje, upewnij się, że użytkownik jest zalogowany w stronę. 
    - Jeśli jest to użytkownik zewnętrzny, upewnij się, że ich zaproszenie zostało zaakceptowane.
    - Jeśli użytkownik istnieje w grupie uprawnień, upewnij się, że adres e-mail jest poprawny.
    - Jeśli adres e-mail użytkownika nie jest ustawiona w tym polu, następnie utworzyć przykładowy alert dla tego użytkownika, co zmusza synchronizacji tego konta użytkownika z profilów użytkownika programu SharePoint do tego zbioru witryn.
 
2. Wiadomości e-mail z przepływów pracy są wysyłane do administratorów zbioru witryn, ale nie do innych użytkowników i wyświetlany jest błąd **HTTP zabrania się <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Zobacz, [Odmowa dostępu podczas wysyłania wiadomości e-mail do grupy programu SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Sprawdź także, że funkcji zbioru witryn **Tryb blokowania uprawnień ograniczony dostęp użytkownika** nie jest aktywne.


## <a name="related-topics"></a>Tematy pokrewne
Czy chcesz spróbować Flow Microsoft w dokumentacji Online programu SharePoint?
- [Utworzyć przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i przepływu](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



---
title: Wiadomość e-mail przepływu pracy nie jest wysyłana
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
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072530"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Wiadomość e-mail przepływu pracy nie jest wysyłana dla listy SharePoint lub biblioteki

1. Wiadomości e-mail z przepływów pracy nie są wysyłane do wszystkich użytkowników lub tylko do konkretnych użytkowników lub jest wyświetlany komunikat o błędzie Nie można wysłać wiadomości e-mail. Upewnij się, że wiadomość **e-mail ma prawidłowego adresata.**

    Sprawdź, czy użytkownik istnieje w grupie uprawnień Wszystkie **osoby** (lista informacji o użytkowniku) dla tego zbioru witryn.  Przykładowy bezpośredni adres URL: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Jeśli użytkownik nie istnieje, upewnij się, że jest zalogowany na stronie. 
    - Jeśli jest to użytkownik zewnętrzny, upewnij się, że jego zaproszenie zostało zaakceptowane.
    - Jeśli użytkownik istnieje w grupie uprawnień, upewnij się, że adres e-mail jest poprawny.
    - Jeśli adres e-mail użytkownika nie został tutaj ustawiony, utwórz dla tego użytkownika przykładowy alert, który wymusza synchronizację tego konta użytkownika z profilów SharePoint z tym zbiorem witryn.
 
2. Wiadomości e-mail z przepływów pracy są wysyłane do administratorów zbioru witryn, ale nie do innych użytkowników i jest wyświetlany błąd HTTP Dostęp zabroniony **<span>dla https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail.**
 

    Zobacz [Odmowa dostępu podczas wysyłania wiadomości e-mail do SharePoint grupy](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Sprawdź też, czy **funkcja** zbioru witryn w trybie blokowania uprawnień użytkownika z ograniczonym dostępem nie jest aktywna.


## <a name="related-topics"></a>Tematy pokrewne
Chcesz wypróbować te Microsoft Flow w SharePoint Online?
- [Tworzenie Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



---
title: Nie jest wysyłana wiadomość e-mail przepływu pracy
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748999"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Nie jest wysyłana wiadomość e-mail przepływu pracy dla listy lub biblioteki programu SharePoint

1. Wiadomości e-mail z przepływów pracy nie są wysyłane do wszystkich użytkowników lub tylko określonych użytkowników lub jest wyświetlany **komunikat o błędzie nie można wysłać wiadomości e-mail. Upewnij się, że wiadomość e-mail ma prawidłowego adresata**.

    Sprawdź, czy użytkownik znajduje się w grupie uprawnienia **wszystkich osób** (liście informacje o użytkowniku) dla tego zbioru witryn.  Przykładowy bezpośredni adres URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Jeśli użytkownik nie istnieje, upewnij się, że użytkownik jest zalogowany na stronie. 
    - Jeśli jest to użytkownik zewnętrzny, upewnij się, że jego zaproszenie zostało zaakceptowane.
    - Jeśli użytkownik znajduje się w grupie uprawnienia, upewnij się, że adres e-mail jest odpowiedni.
    - Jeśli adres e-mail użytkownika nie jest ustawiony w tym miejscu, Utwórz przykładowy alert dla tego użytkownika, który wymusza synchronizację tego konta użytkownika z profilów użytkowników programu SharePoint z tym zbiorem witryn.
 
2. Wiadomości e-mail z przepływów pracy są wysyłane do administratorów zbioru witryn, ale nie do innych użytkowników i widzą błąd **http zabroniony na <span>https:</span>//URL/_vti_bin/Client.XVC.Sp.Utilities.Utility.SendEmail**.
 

    Zobacz [odmowa dostępu podczas wysyłania wiadomości e-mail do grupy programu SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Upewnij się też, że funkcja zbioru witryn **tryb blokowania uprawnień użytkownika z ograniczonym dostępem** jest nieaktywna.


## <a name="related-topics"></a>Tematy pokrewne
Chcesz wypróbować przepływ pracy Microsoft w usłudze SharePoint Online?
- [Utwórz przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Program SharePoint i przepływ](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



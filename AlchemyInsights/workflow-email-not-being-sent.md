---
title: E-mail przepływu pracy nie jest wysyłany
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049383"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Wiadomości e-mail przepływu pracy nie są wysyłane do listy programu SharePoint lub biblioteki

1. Wiadomości e-mail z przepływów pracy nie są wysyłane do wszystkich użytkowników lub tylko określonych użytkowników lub zostanie wyświetlony błąd **nie można wysłać wiadomości e-mail. Upewnij się, że wiadomość e-mail ma prawidłowego adresata**.

    Sprawdź, czy użytkownik istnieje w grupie uprawnienia **wszystkich osób** (lista informacji o użytkowniczek) dla tego zbioru witryn.  Przykładowy bezpośredni adres URL:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/People.aspx? MembershipGroupId = 0

    - Jeśli użytkownik nie istnieje, upewnij się, że użytkownik jest zalogowany na stronie. 
    - Jeśli jest to użytkownik zewnętrzny, upewnij się, że zaproszenie zostało zaakceptowane.
    - Jeśli użytkownik nie istnieje w grupie uprawnień, upewnij się, że adres e-mail jest poprawny.
    - Jeśli adres e-mail użytkowników nie jest ustawiony w tym miejscu, Utwórz przykładowy alert dla tego użytkownika, który wymusza synchronizację tego konta użytkownika z profilów użytkowników programu SharePoint do tego zbioru witryn.
 
2. Wiadomości e-mail z przepływów pracy są wysyłane do administratorów zbioru witryn, ale nie do innych użytkowników i Zobacz błąd **http zabronione <span>https:</span>/URL/_vti_bin/Client.XVC.Sp.Utilities.Utility.SendEmail**.
 

    Zobacz [odmowa dostępu podczas wysyłania wiadomości e-mail do grupy programu SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Ponadto sprawdź, czy funkcja zbioru witryn **trybu blokowania uprawnień ograniczonego dostępu użytkownika** nie jest aktywna.


## <a name="related-topics"></a>Tematy pokrewne
Chcesz wypróbować usługi Microsoft Flow w usłudze SharePoint Online?
- [Utwórz przepływ](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i przepływu](https://flow.microsoft.com/blog/sharepoint-and-flow/) 



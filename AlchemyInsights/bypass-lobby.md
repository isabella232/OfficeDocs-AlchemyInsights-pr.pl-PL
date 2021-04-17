---
title: Pomijanie poczekalni
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820044"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrolowanie ustawień poczekalni i poziomu uczestnictwa w aplikacji Teams

Jeśli chcesz zezwolić wszystkim, w tym użytkownikom korzystającym z połączeń telefonicznych, zewnętrznych i anonimowych, na ominięcie poczekalni, użyj programu PowerShell, aby wykonać to zadanie. Oto przykład modyfikowania globalnych zasad spotkań dla organizacji.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

To polecenie cmdlet obecnie wymaga użycia modułu programu Skype dla firm PowerShell. Aby skonfigurować używanie tego polecenia cmdlet, zobacz [Zarządzanie zasadami za pomocą programu PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Po skonfigurowaniu zasad należy je zastosować do użytkowników. lub, jeśli zmodyfikowasz zasady globalne, zostaną one automatycznie stosowane do użytkowników. W przypadku każdej zmiany zasad należy zaczekać od co najmniej 4 godzin do **24** godzin na ich skutek. 

Przed wprowadzeniem tych zmian należy zapoznać się z poniższymi dokumentami, aby dokładnie zrozumieć, na czym to pozwala.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Opis kontrolek zasad poczekalni spotkania w u teamsie

Te ustawienia kontrolują, którzy uczestnicy spotkania czekają w poczekalni przed wpuszczeniem na spotkanie, oraz jaki jest dozwolony poziom uczestnictwa w spotkaniu. Za pomocą programu PowerShell możesz zaktualizować ustawienia zasad spotkania, które nie zostały jeszcze zaimplementowane (oznaczone jako "wkrótce") w centrum administracyjnym usługi Teams. Poniżej znajduje się przykładowe polecenie cmdlet programu PowerShell, które umożliwia wszystkim użytkownikom pomijanie poczekalni.

- [Automatyczne wpuszczanie osób](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) to zasady per-organizer, które sterują tym, czy osoby mogą dołączać do spotkania bezpośrednio, czy czekać w poczekalni na wpuszczenie przez uwierzytelnionego użytkownika.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Zezwalaj osobom anonimowym na rozpoczynanie spotkania to zasady dla organizatorów, które sterują tym, czy anonimowe osoby, w tym B2B i użytkownicy federacyjni, mogą dołączać do spotkania użytkownika bez uwierzytelnionego użytkownika z organizacji w obecności.

- Zezwalaj użytkownikom korzystającym z połączeń telefonicznych na ominięcie poczekalni [(już](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **wkrótce)** to zasady dotyczące  per-organizera, które sterują tym, czy osoby dołączane telefonicznie mogą dołączać do spotkania bezpośrednio, czy czekać w poczekalni bez względu na ustawienie Automatycznie wpuszczaj osoby.

- Zezwalaj organizatorom na zastępowanie ustawień poczekalni [(już](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **wkrótce)** to zasady dla organizatorów,  które sterują tym, czy organizator spotkania może zastąpić ustawienia poczekalni ustawione przez administratora w polach Automatyczne wpuszczanie osób i Zezwalaj użytkownikom korzystającym z poczekalni na pomijanie poczekalni podczas planowania nowego spotkania. 

**Uwaga:** Przeczytaj [Zarządzanie zasadami spotkań w aplikacji Teams,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) aby uzyskać pełne omówienie zasad spotkania w aplikacji Microsoft Teams.

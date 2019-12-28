---
title: Obejście lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889092"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrolowanie ustawień lobby i poziomu uczestnictwa w zespołach

Jeśli chcesz zezwolić wszystkim, w tym telefonowania, zewnętrzni i anonimowi użytkownicy, aby **ominąć lobby**, użyj programu PowerShell, aby wykonać to zadanie. Oto przykład modyfikowania globalne zasady spotkania dla organizacji.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

To polecenie cmdlet obecnie wymaga użycia programu Skype dla modułu Business PowerShell. Aby uzyskać skonfigurowane do używania tego polecenia cmdlet, zapoznaj się z [zasadami zarządzania za pomocą programu PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Po skonfigurowaniu zasad należy ją zastosować do użytkowników; lub, jeśli zmodyfikowano politykę globalną, będzie ona automatycznie stosowana do użytkowników. W przypadku każdej zmiany zasad należy poczekać co najmniej **4 godziny do 24 godzin** , aby zasady zostały uwzględnione. 

Przed wprowadzeniem tych zmian należy zapoznać się z poniższą dokumentacją, aby dokładnie zrozumieć, co to pozwala.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Opis formantów zasad lobby spotkań zespołów

Te ustawienia kontrolują, którzy uczestnicy spotkania czekają w lobby, zanim zostaną przyjęci na spotkanie i poziom uczestnictwa, jaki są dozwolone na spotkaniu. Można użyć programu PowerShell, aby zaktualizować ustawienia zasad spotkania, które nie zostały jeszcze wdrożone (etykietą "wkrótce") w centrum administracyjnym zespołów. Poniżej przedstawiono przykładowe polecenie cmdlet programu PowerShell, które pozwala wszystkim użytkownikom ominąć lobby.

- [Automatycznie przyznać](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , że ludzie to zasady na organizatora, który kontroluje, czy ludzie przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, dopóki nie zostaną dopuszczone przez uwierzytelnionego użytkownika.

- [Zezwalaj osobom anonimowym na rozpoczęcie spotkania](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) to zasada na organizatora, która kontroluje, czy osoby anonimowe, w tym B2B i użytkownicy federacyjni, mogą przyłączyć się do spotkania użytkownika bez uwierzytelnionego użytkownika z organizacji w obecności.

- [Zezwalaj użytkownikom telefonowania na ominięcie lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**wkrótce**) jest to zasada dla organizatora, która kontroluje, czy osoby, które telefonują przez telefon przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, niezależnie od **automatycznie przyznać ustawienie osób** .

- [Pozwól organizatorom na zastąpienie ustawień lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(wkrótce**) jest to zasada dla organizatora, która kontroluje, czy organizator spotkania może zastąpić ustawienia lobby, które admin ustawiają **automatycznie przyznać ludziom** i **zezwolić użytkownikom telefonowania ominąć lobby** podczas planowania nowego spotkania.

**Uwaga:** Przeczytaj [Zarządzanie zasadami spotkania w zespołach](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , aby uzyskać pełny przegląd zasad dotyczących spotkań w programie Microsoft Teams.

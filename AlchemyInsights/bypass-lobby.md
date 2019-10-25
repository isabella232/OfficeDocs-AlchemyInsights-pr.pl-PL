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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654266"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Sterowanie ustawieniami lobby i poziomem uczestnictwa

Jeśli chcesz zezwolić wszystkim, w tym telefonowania, zewnętrzni i anonimowi użytkownicy ominąć lobby, można użyć programu PowerShell, aby to zrobić. Oto przykład modyfikowania globalnych zasad spotkania dla organizacji:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

To polecenie cmdlet obecnie wymaga użycia programu Skype dla modułu Business PowerShell. Aby uzyskać Instalator, aby użyć tego polecenia cmdlet, zapoznaj się z [zasadami zarządzania za pomocą programu PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Można skonfigurować nowe zasady, które następnie należy zastosować do użytkowników. W przypadku zmodyfikowania zasad globalnych będzie ona automatycznie stosowana do użytkowników. W przypadku każdej zmiany zasad należy poczekać co najmniej 4 godziny i do 24 godzin, aby zasady zostały uwzględnione.

Przed wprowadzeniem tych zmian należy zapoznać się z poniższą dokumentacją, aby dokładnie zrozumieć, co to pozwala.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Opis formantów zasad lobby spotkań zespołów

- [Automatycznie przyznać](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , że ludzie to zasady na organizatora, który kontroluje, czy ludzie przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, dopóki nie zostaną dopuszczone przez uwierzytelnionego użytkownika.

- [Zezwalaj osobom anonimowym na rozpoczęcie spotkania](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) to zasada na organizatora, która kontroluje, czy osoby anonimowe, w tym B2B i użytkownicy federacyjni, mogą przyłączyć się do spotkania użytkownika bez uwierzytelnionego użytkownika z organizacji w obecności.

- [Zezwalaj użytkownikom telefonowania na ominięcie lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**wkrótce**) jest to zasada dla organizatora, która kontroluje, czy osoby, które telefonują przez telefon przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, niezależnie od **automatycznie przyznać ustawienie osób** .

- [Pozwól organizatorom na zastąpienie ustawień lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(wkrótce**) jest to zasada dla organizatora, która kontroluje, czy organizator spotkania może zastąpić ustawienia lobby, które admin ustawiają **automatycznie przyznać ludziom** i zezwolić na **telefonowania użytkownikom na ominięcie lobby** podczas planowania nowego spotkania.

**Uwaga:** Przeczytaj [Zarządzanie zasadami spotkania w zespołach](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , aby uzyskać pełny przegląd zasad dotyczących spotkań w programie Microsoft Teams.

---
title: Obejdź poczekalnię
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684960"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Sterowanie ustawieniami poczekalni i poziomem uczestnictwa w aplikacji Teams

Jeśli chcesz zezwolić wszystkim, w tym użytkownikom telefonicznym, zewnętrznym i anonimowym, na **pomijanie poczekalni**, użyj programu PowerShell, aby wykonać to zadanie. Oto przykładowa modyfikacja globalnych zasad spotkań dla organizacji.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

To polecenie cmdlet wymaga obecnie korzystania z modułu programu PowerShell w programie Skype dla firm. Aby skonfigurować korzystanie z tego polecenia cmdlet, zobacz [Zarządzanie zasadami za pomocą programu PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Po skonfigurowaniu zasad trzeba je zastosować do użytkowników; Jeśli zasady globalne zostały zmodyfikowane, będą one automatycznie stosowane do użytkowników. W przypadku każdej zmiany zasad musisz poczekać co najmniej **4 godziny na 24 godziny** , aby zasady zostały zastosowane. 

Przed wprowadzeniem tych zmian należy zapoznać się z poniższą dokumentacją.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Opis formantów zasad poczekalni spotkań aplikacji Teams

Te ustawienia kontrolują, które uczestnicy spotkania czekają na poczekalnię, zanim zostaną przyjęte na spotkanie i poziom uczestnictwa w spotkaniu. Za pomocą programu PowerShell można aktualizować ustawienia zasad spotkań, które nie zostały jeszcze zaimplementowane ("już wkrótce") w centrum administracyjnym aplikacji Teams. Poniżej znajduje się przykładowe polecenie cmdlet programu PowerShell, które umożliwia wszystkim użytkownikom pomijanie poczekalni.

- [Automatyczne przyjmowanie osób](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) to zasady dotyczące każdego organizatora, które kontrolują, czy osoby dołączające do spotkania bezpośrednio lub oczekują w poczekalni do momentu ich otrzymania przez uwierzytelnionego użytkownika.

- [Zezwól anonimowym użytkownikom na Rozpoczynanie spotkania](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) to zasady dotyczące każdego organizatora, które kontrolują, czy anonimowe osoby, w tym użytkownicy typu B2B i federacyjnego, mogą dołączać do spotkania użytkownika bez uwierzytelnionego użytkownika w organizacji w ramach uczestnictwa.

- [Zezwalaj użytkownikom telefonowania na pomijanie poczekalni](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**już wkrótce**) jest to zasada dla każdego organizatora, która kontroluje, czy osoby, które wybierają numery telefoniczne bezpośrednio do spotkania lub oczekują w poczekalni bez względu na ustawienie automatyczne akceptowanie **osób** .

- [Zezwól organizatorom na zastępowanie ustawień lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**już wkrótce**) to zasady dotyczące organizatora określające, czy organizator spotkania może zastępować ustawienia lobby, które administrator ustawił w polu **automatycznie dopuścić osoby** i **zezwala użytkownikom na połączenia z pominięciem poczekalni** podczas planowania nowego spotkania.

**Uwaga:** Przeczytaj temat [Zarządzanie zasadami dotyczącymi spotkań w aplikacji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , aby zapoznać się z pełnym omówieniem zasad spotkań aplikacji Microsoft Teams.

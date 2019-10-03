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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376765"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Sterowanie ustawieniami lobby i poziomem uczestnictwa

Te ustawienia kontrolują, którzy uczestnicy spotkania czekają w lobby, zanim zostaną przyjęci na spotkanie i poziom uczestnictwa, jaki są dozwolone na spotkaniu. Można użyć programu PowerShell, aby zaktualizować ustawienia zasad spotkania, które nie zostały jeszcze wdrożone (oznaczone jako "wkrótce") w centrum administracyjnym zespołów.  Poniżej przedstawiono przykładowe polecenie cmdlet programu PowerShell, które pozwala wszystkim użytkownikom ominąć lobby.  

- [Automatycznie przyznać](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , że ludzie to zasady na organizatora, który kontroluje, czy ludzie przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, dopóki nie zostaną dopuszczone przez uwierzytelnionego użytkownika.

- [Zezwalaj osobom anonimowym na rozpoczęcie spotkania](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) to zasada na organizatora, która kontroluje, czy osoby anonimowe, w tym B2B i użytkownicy federacyjni, mogą przyłączyć się do spotkania użytkownika bez uwierzytelnionego użytkownika z organizacji w obecności.

- [Zezwalaj użytkownikom telefonowania na ominięcie lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**wkrótce**) jest to zasada dla organizatora, która kontroluje, czy osoby, które telefonują przez telefon przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, niezależnie od **automatycznie przyznać ustawienie osób** .

- [Pozwól organizatorom na zastąpienie ustawień lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(wkrótce**) jest to zasada dla organizatora, która kontroluje, czy organizator spotkania może zastąpić ustawienia lobby, które admin ustawiają **automatycznie przyznać ludziom** i zezwolić na **telefonowania użytkownikom na ominięcie lobby** podczas planowania nowego spotkania.

**Uwaga:** Przeczytaj [Zarządzanie zasadami spotkania w zespołach](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , aby uzyskać pełny przegląd zasad dotyczących spotkań w programie Microsoft Teams. 


**Przykład programu Powershellpowershell example**

Jeśli chcesz zezwolić wszystkim, w tym użytkownikom zewnętrznym lub anonimowym, ominąć lobby, możesz również użyć programu PowerShell, aby wykonać to zadanie.  Oto przykład modyfikowania globalne zasady spotkania dla organizacji.   

(Przed wprowadzeniem tych zmian zapoznaj się z dokumentacją powyżej, aby dokładnie zrozumieć, co to pozwala).

Zestaw CsTeamsMeetingPolicy-tożsamość globalny-AutoAdmittedUsers "Wszyscy"-AllowPSTNUsersToBypassLobby $True

Aby uzyskać więcej informacji, zobacz [zestaw CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).

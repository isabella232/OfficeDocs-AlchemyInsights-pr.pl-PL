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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="c42fb-102">Sterowanie ustawieniami lobby i poziomem uczestnictwa</span><span class="sxs-lookup"><span data-stu-id="c42fb-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="c42fb-103">Te ustawienia kontrolują, którzy uczestnicy spotkania czekają w lobby, zanim zostaną przyjęci na spotkanie i poziom uczestnictwa, jaki są dozwolone na spotkaniu.</span><span class="sxs-lookup"><span data-stu-id="c42fb-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="c42fb-104">Można użyć programu PowerShell, aby zaktualizować ustawienia zasad spotkania, które nie zostały jeszcze wdrożone (oznaczone jako "wkrótce") w centrum administracyjnym zespołów.</span><span class="sxs-lookup"><span data-stu-id="c42fb-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="c42fb-105">Poniżej przedstawiono przykładowe polecenie cmdlet programu PowerShell, które pozwala wszystkim użytkownikom ominąć lobby.</span><span class="sxs-lookup"><span data-stu-id="c42fb-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="c42fb-106">[Automatycznie przyznać](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , że ludzie to zasady na organizatora, który kontroluje, czy ludzie przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, dopóki nie zostaną dopuszczone przez uwierzytelnionego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="c42fb-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="c42fb-107">[Zezwalaj osobom anonimowym na rozpoczęcie spotkania](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) to zasada na organizatora, która kontroluje, czy osoby anonimowe, w tym B2B i użytkownicy federacyjni, mogą przyłączyć się do spotkania użytkownika bez uwierzytelnionego użytkownika z organizacji w obecności.</span><span class="sxs-lookup"><span data-stu-id="c42fb-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="c42fb-108">[Zezwalaj użytkownikom telefonowania na ominięcie lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**wkrótce**) jest to zasada dla organizatora, która kontroluje, czy osoby, które telefonują przez telefon przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, niezależnie od **automatycznie przyznać ustawienie osób** .</span><span class="sxs-lookup"><span data-stu-id="c42fb-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="c42fb-109">[Pozwól organizatorom na zastąpienie ustawień lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(wkrótce**) jest to zasada dla organizatora, która kontroluje, czy organizator spotkania może zastąpić ustawienia lobby, które admin ustawiają **automatycznie przyznać ludziom** i zezwolić na **telefonowania użytkownikom na ominięcie lobby** podczas planowania nowego spotkania.</span><span class="sxs-lookup"><span data-stu-id="c42fb-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="c42fb-110">**Uwaga:** Przeczytaj [Zarządzanie zasadami spotkania w zespołach](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , aby uzyskać pełny przegląd zasad dotyczących spotkań w programie Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c42fb-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="c42fb-111">**Przykład programu Powershellpowershell example**</span><span class="sxs-lookup"><span data-stu-id="c42fb-111">**PowerShell example**</span></span>

<span data-ttu-id="c42fb-112">Jeśli chcesz zezwolić wszystkim, w tym użytkownikom zewnętrznym lub anonimowym, ominąć lobby, możesz również użyć programu PowerShell, aby wykonać to zadanie.</span><span class="sxs-lookup"><span data-stu-id="c42fb-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="c42fb-113">Oto przykład modyfikowania globalne zasady spotkania dla organizacji.</span><span class="sxs-lookup"><span data-stu-id="c42fb-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="c42fb-114">(Przed wprowadzeniem tych zmian zapoznaj się z dokumentacją powyżej, aby dokładnie zrozumieć, co to pozwala).</span><span class="sxs-lookup"><span data-stu-id="c42fb-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="c42fb-115">Zestaw CsTeamsMeetingPolicy-tożsamość globalny-AutoAdmittedUsers "Wszyscy"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="c42fb-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="c42fb-116">Aby uzyskać więcej informacji, zobacz [zestaw CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="c42fb-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>

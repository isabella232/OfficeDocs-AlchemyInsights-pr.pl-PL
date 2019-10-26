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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/25/2019
ms.locfileid: "37654266"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="3c84b-102">Sterowanie ustawieniami lobby i poziomem uczestnictwa</span><span class="sxs-lookup"><span data-stu-id="3c84b-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="3c84b-103">Jeśli chcesz zezwolić wszystkim, w tym telefonowania, zewnętrzni i anonimowi użytkownicy ominąć lobby, można użyć programu PowerShell, aby to zrobić.</span><span class="sxs-lookup"><span data-stu-id="3c84b-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="3c84b-104">Oto przykład modyfikowania globalnych zasad spotkania dla organizacji:</span><span class="sxs-lookup"><span data-stu-id="3c84b-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="3c84b-105">To polecenie cmdlet obecnie wymaga użycia programu Skype dla modułu Business PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3c84b-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="3c84b-106">Aby uzyskać Instalator, aby użyć tego polecenia cmdlet, zapoznaj się z [zasadami zarządzania za pomocą programu PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="3c84b-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="3c84b-107">Można skonfigurować nowe zasady, które następnie należy zastosować do użytkowników.</span><span class="sxs-lookup"><span data-stu-id="3c84b-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="3c84b-108">W przypadku zmodyfikowania zasad globalnych będzie ona automatycznie stosowana do użytkowników.</span><span class="sxs-lookup"><span data-stu-id="3c84b-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="3c84b-109">W przypadku każdej zmiany zasad należy poczekać co najmniej 4 godziny i do 24 godzin, aby zasady zostały uwzględnione.</span><span class="sxs-lookup"><span data-stu-id="3c84b-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="3c84b-110">Przed wprowadzeniem tych zmian należy zapoznać się z poniższą dokumentacją, aby dokładnie zrozumieć, co to pozwala.</span><span class="sxs-lookup"><span data-stu-id="3c84b-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="3c84b-111">Opis formantów zasad lobby spotkań zespołów</span><span class="sxs-lookup"><span data-stu-id="3c84b-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="3c84b-112">[Automatycznie przyznać](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , że ludzie to zasady na organizatora, który kontroluje, czy ludzie przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, dopóki nie zostaną dopuszczone przez uwierzytelnionego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="3c84b-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="3c84b-113">[Zezwalaj osobom anonimowym na rozpoczęcie spotkania](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) to zasada na organizatora, która kontroluje, czy osoby anonimowe, w tym B2B i użytkownicy federacyjni, mogą przyłączyć się do spotkania użytkownika bez uwierzytelnionego użytkownika z organizacji w obecności.</span><span class="sxs-lookup"><span data-stu-id="3c84b-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="3c84b-114">[Zezwalaj użytkownikom telefonowania na ominięcie lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**wkrótce**) jest to zasada dla organizatora, która kontroluje, czy osoby, które telefonują przez telefon przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, niezależnie od **automatycznie przyznać ustawienie osób** .</span><span class="sxs-lookup"><span data-stu-id="3c84b-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="3c84b-115">[Pozwól organizatorom na zastąpienie ustawień lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(wkrótce**) jest to zasada dla organizatora, która kontroluje, czy organizator spotkania może zastąpić ustawienia lobby, które admin ustawiają **automatycznie przyznać ludziom** i zezwolić na **telefonowania użytkownikom na ominięcie lobby** podczas planowania nowego spotkania.</span><span class="sxs-lookup"><span data-stu-id="3c84b-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="3c84b-116">**Uwaga:** Przeczytaj [Zarządzanie zasadami spotkania w zespołach](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) , aby uzyskać pełny przegląd zasad dotyczących spotkań w programie Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3c84b-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>

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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="6d47f-102">Kontrolowanie ustawień poczekalni i poziomu uczestnictwa w aplikacji Teams</span><span class="sxs-lookup"><span data-stu-id="6d47f-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="6d47f-103">Jeśli chcesz zezwolić wszystkim, w tym użytkownikom korzystającym z połączeń telefonicznych, zewnętrznych i anonimowych, na ominięcie poczekalni, użyj programu PowerShell, aby wykonać to zadanie.</span><span class="sxs-lookup"><span data-stu-id="6d47f-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="6d47f-104">Oto przykład modyfikowania globalnych zasad spotkań dla organizacji.</span><span class="sxs-lookup"><span data-stu-id="6d47f-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="6d47f-105">To polecenie cmdlet obecnie wymaga użycia modułu programu Skype dla firm PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6d47f-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="6d47f-106">Aby skonfigurować używanie tego polecenia cmdlet, zobacz [Zarządzanie zasadami za pomocą programu PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="6d47f-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="6d47f-107">Po skonfigurowaniu zasad należy je zastosować do użytkowników. lub, jeśli zmodyfikowasz zasady globalne, zostaną one automatycznie stosowane do użytkowników.</span><span class="sxs-lookup"><span data-stu-id="6d47f-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="6d47f-108">W przypadku każdej zmiany zasad należy zaczekać od co najmniej 4 godzin do **24** godzin na ich skutek.</span><span class="sxs-lookup"><span data-stu-id="6d47f-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="6d47f-109">Przed wprowadzeniem tych zmian należy zapoznać się z poniższymi dokumentami, aby dokładnie zrozumieć, na czym to pozwala.</span><span class="sxs-lookup"><span data-stu-id="6d47f-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="6d47f-110">Opis kontrolek zasad poczekalni spotkania w u teamsie</span><span class="sxs-lookup"><span data-stu-id="6d47f-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="6d47f-111">Te ustawienia kontrolują, którzy uczestnicy spotkania czekają w poczekalni przed wpuszczeniem na spotkanie, oraz jaki jest dozwolony poziom uczestnictwa w spotkaniu.</span><span class="sxs-lookup"><span data-stu-id="6d47f-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="6d47f-112">Za pomocą programu PowerShell możesz zaktualizować ustawienia zasad spotkania, które nie zostały jeszcze zaimplementowane (oznaczone jako "wkrótce") w centrum administracyjnym usługi Teams.</span><span class="sxs-lookup"><span data-stu-id="6d47f-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="6d47f-113">Poniżej znajduje się przykładowe polecenie cmdlet programu PowerShell, które umożliwia wszystkim użytkownikom pomijanie poczekalni.</span><span class="sxs-lookup"><span data-stu-id="6d47f-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="6d47f-114">[Automatyczne wpuszczanie osób](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) to zasady per-organizer, które sterują tym, czy osoby mogą dołączać do spotkania bezpośrednio, czy czekać w poczekalni na wpuszczenie przez uwierzytelnionego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6d47f-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="6d47f-115">[](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Zezwalaj osobom anonimowym na rozpoczynanie spotkania to zasady dla organizatorów, które sterują tym, czy anonimowe osoby, w tym B2B i użytkownicy federacyjni, mogą dołączać do spotkania użytkownika bez uwierzytelnionego użytkownika z organizacji w obecności.</span><span class="sxs-lookup"><span data-stu-id="6d47f-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="6d47f-116">Zezwalaj użytkownikom korzystającym z połączeń telefonicznych na ominięcie poczekalni [(już](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **wkrótce)** to zasady dotyczące  per-organizera, które sterują tym, czy osoby dołączane telefonicznie mogą dołączać do spotkania bezpośrednio, czy czekać w poczekalni bez względu na ustawienie Automatycznie wpuszczaj osoby.</span><span class="sxs-lookup"><span data-stu-id="6d47f-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="6d47f-117">Zezwalaj organizatorom na zastępowanie ustawień poczekalni [(już](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **wkrótce)** to zasady dla organizatorów,  które sterują tym, czy organizator spotkania może zastąpić ustawienia poczekalni ustawione przez administratora w polach Automatyczne wpuszczanie osób i Zezwalaj użytkownikom korzystającym z poczekalni na pomijanie poczekalni podczas planowania nowego spotkania. </span><span class="sxs-lookup"><span data-stu-id="6d47f-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="6d47f-118">**Uwaga:** Przeczytaj [Zarządzanie zasadami spotkań w aplikacji Teams,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) aby uzyskać pełne omówienie zasad spotkania w aplikacji Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6d47f-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>

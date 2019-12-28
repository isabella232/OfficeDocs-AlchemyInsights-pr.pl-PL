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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="62c90-102">Kontrolowanie ustawień lobby i poziomu uczestnictwa w zespołach</span><span class="sxs-lookup"><span data-stu-id="62c90-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="62c90-103">Jeśli chcesz zezwolić wszystkim, w tym telefonowania, zewnętrzni i anonimowi użytkownicy, aby **ominąć lobby**, użyj programu PowerShell, aby wykonać to zadanie.</span><span class="sxs-lookup"><span data-stu-id="62c90-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="62c90-104">Oto przykład modyfikowania globalne zasady spotkania dla organizacji.</span><span class="sxs-lookup"><span data-stu-id="62c90-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="62c90-105">To polecenie cmdlet obecnie wymaga użycia programu Skype dla modułu Business PowerShell.</span><span class="sxs-lookup"><span data-stu-id="62c90-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="62c90-106">Aby uzyskać skonfigurowane do używania tego polecenia cmdlet, zapoznaj się z [zasadami zarządzania za pomocą programu PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="62c90-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="62c90-107">Po skonfigurowaniu zasad należy ją zastosować do użytkowników; lub, jeśli zmodyfikowano politykę globalną, będzie ona automatycznie stosowana do użytkowników.</span><span class="sxs-lookup"><span data-stu-id="62c90-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="62c90-108">W przypadku każdej zmiany zasad należy poczekać co najmniej **4 godziny do 24 godzin** , aby zasady zostały uwzględnione.</span><span class="sxs-lookup"><span data-stu-id="62c90-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="62c90-109">Przed wprowadzeniem tych zmian należy zapoznać się z poniższą dokumentacją, aby dokładnie zrozumieć, co to pozwala.</span><span class="sxs-lookup"><span data-stu-id="62c90-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="62c90-110">Opis formantów zasad lobby spotkań zespołów</span><span class="sxs-lookup"><span data-stu-id="62c90-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="62c90-111">Te ustawienia kontrolują, którzy uczestnicy spotkania czekają w lobby, zanim zostaną przyjęci na spotkanie i poziom uczestnictwa, jaki są dozwolone na spotkaniu.</span><span class="sxs-lookup"><span data-stu-id="62c90-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="62c90-112">Można użyć programu PowerShell, aby zaktualizować ustawienia zasad spotkania, które nie zostały jeszcze wdrożone (etykietą "wkrótce") w centrum administracyjnym zespołów.</span><span class="sxs-lookup"><span data-stu-id="62c90-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="62c90-113">Poniżej przedstawiono przykładowe polecenie cmdlet programu PowerShell, które pozwala wszystkim użytkownikom ominąć lobby.</span><span class="sxs-lookup"><span data-stu-id="62c90-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="62c90-114">[Automatycznie przyznać](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , że ludzie to zasady na organizatora, który kontroluje, czy ludzie przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, dopóki nie zostaną dopuszczone przez uwierzytelnionego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="62c90-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="62c90-115">[Zezwalaj osobom anonimowym na rozpoczęcie spotkania](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) to zasada na organizatora, która kontroluje, czy osoby anonimowe, w tym B2B i użytkownicy federacyjni, mogą przyłączyć się do spotkania użytkownika bez uwierzytelnionego użytkownika z organizacji w obecności.</span><span class="sxs-lookup"><span data-stu-id="62c90-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="62c90-116">[Zezwalaj użytkownikom telefonowania na ominięcie lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**wkrótce**) jest to zasada dla organizatora, która kontroluje, czy osoby, które telefonują przez telefon przyłączyć się do spotkania bezpośrednio lub poczekać w lobby, niezależnie od **automatycznie przyznać ustawienie osób** .</span><span class="sxs-lookup"><span data-stu-id="62c90-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="62c90-117">[Pozwól organizatorom na zastąpienie ustawień lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(wkrótce**) jest to zasada dla organizatora, która kontroluje, czy organizator spotkania może zastąpić ustawienia lobby, które admin ustawiają **automatycznie przyznać ludziom** i **zezwolić użytkownikom telefonowania ominąć lobby** podczas planowania nowego spotkania.</span><span class="sxs-lookup"><span data-stu-id="62c90-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="62c90-118">**Uwaga:** Przeczytaj [Zarządzanie zasadami spotkania w zespołach](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , aby uzyskać pełny przegląd zasad dotyczących spotkań w programie Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="62c90-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>

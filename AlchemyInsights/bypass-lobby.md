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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="28013-102">Sterowanie ustawieniami poczekalni i poziomem uczestnictwa w aplikacji Teams</span><span class="sxs-lookup"><span data-stu-id="28013-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="28013-103">Jeśli chcesz zezwolić wszystkim, w tym użytkownikom telefonicznym, zewnętrznym i anonimowym, na **pomijanie poczekalni**, użyj programu PowerShell, aby wykonać to zadanie.</span><span class="sxs-lookup"><span data-stu-id="28013-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="28013-104">Oto przykładowa modyfikacja globalnych zasad spotkań dla organizacji.</span><span class="sxs-lookup"><span data-stu-id="28013-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="28013-105">To polecenie cmdlet wymaga obecnie korzystania z modułu programu PowerShell w programie Skype dla firm.</span><span class="sxs-lookup"><span data-stu-id="28013-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="28013-106">Aby skonfigurować korzystanie z tego polecenia cmdlet, zobacz [Zarządzanie zasadami za pomocą programu PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="28013-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="28013-107">Po skonfigurowaniu zasad trzeba je zastosować do użytkowników; Jeśli zasady globalne zostały zmodyfikowane, będą one automatycznie stosowane do użytkowników.</span><span class="sxs-lookup"><span data-stu-id="28013-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="28013-108">W przypadku każdej zmiany zasad musisz poczekać co najmniej **4 godziny na 24 godziny** , aby zasady zostały zastosowane.</span><span class="sxs-lookup"><span data-stu-id="28013-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="28013-109">Przed wprowadzeniem tych zmian należy zapoznać się z poniższą dokumentacją.</span><span class="sxs-lookup"><span data-stu-id="28013-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="28013-110">Opis formantów zasad poczekalni spotkań aplikacji Teams</span><span class="sxs-lookup"><span data-stu-id="28013-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="28013-111">Te ustawienia kontrolują, które uczestnicy spotkania czekają na poczekalnię, zanim zostaną przyjęte na spotkanie i poziom uczestnictwa w spotkaniu.</span><span class="sxs-lookup"><span data-stu-id="28013-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="28013-112">Za pomocą programu PowerShell można aktualizować ustawienia zasad spotkań, które nie zostały jeszcze zaimplementowane ("już wkrótce") w centrum administracyjnym aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="28013-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="28013-113">Poniżej znajduje się przykładowe polecenie cmdlet programu PowerShell, które umożliwia wszystkim użytkownikom pomijanie poczekalni.</span><span class="sxs-lookup"><span data-stu-id="28013-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="28013-114">[Automatyczne przyjmowanie osób](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) to zasady dotyczące każdego organizatora, które kontrolują, czy osoby dołączające do spotkania bezpośrednio lub oczekują w poczekalni do momentu ich otrzymania przez uwierzytelnionego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="28013-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="28013-115">[Zezwól anonimowym użytkownikom na Rozpoczynanie spotkania](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) to zasady dotyczące każdego organizatora, które kontrolują, czy anonimowe osoby, w tym użytkownicy typu B2B i federacyjnego, mogą dołączać do spotkania użytkownika bez uwierzytelnionego użytkownika w organizacji w ramach uczestnictwa.</span><span class="sxs-lookup"><span data-stu-id="28013-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="28013-116">[Zezwalaj użytkownikom telefonowania na pomijanie poczekalni](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**już wkrótce**) jest to zasada dla każdego organizatora, która kontroluje, czy osoby, które wybierają numery telefoniczne bezpośrednio do spotkania lub oczekują w poczekalni bez względu na ustawienie automatyczne akceptowanie **osób** .</span><span class="sxs-lookup"><span data-stu-id="28013-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="28013-117">[Zezwól organizatorom na zastępowanie ustawień lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**już wkrótce**) to zasady dotyczące organizatora określające, czy organizator spotkania może zastępować ustawienia lobby, które administrator ustawił w polu **automatycznie dopuścić osoby** i **zezwala użytkownikom na połączenia z pominięciem poczekalni** podczas planowania nowego spotkania.</span><span class="sxs-lookup"><span data-stu-id="28013-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="28013-118">**Uwaga:** Przeczytaj temat [Zarządzanie zasadami dotyczącymi spotkań w aplikacji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , aby zapoznać się z pełnym omówieniem zasad spotkań aplikacji Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="28013-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>

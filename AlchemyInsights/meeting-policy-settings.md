---
title: Ustawienia zasad spotkania
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042854"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="6c4a8-102">Zarządzanie zasadami spotkań w usłudze Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6c4a8-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="6c4a8-103">**Uwaga: Wprowadzenie zmian zasad dla użytkowników może potrwać do 24 godzin.**</span><span class="sxs-lookup"><span data-stu-id="6c4a8-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="6c4a8-104">Może nie być możliwe natychmiastowe wprowadzenie zmian w nowo utworzonych zasadach; poczekaj 4 godziny i spróbuj ponownie zmodyfikować nowo utworzone zasady.</span><span class="sxs-lookup"><span data-stu-id="6c4a8-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="6c4a8-105">Zasady spotkania służą do kontrolowania funkcji dostępnych dla uczestników spotkania na spotkania, które są zaplanowane przez użytkowników w organizacji.</span><span class="sxs-lookup"><span data-stu-id="6c4a8-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="6c4a8-106">Niektóre funkcje zasad spotkania mogą nie zostać jeszcze zaimplementowane w centrum administracyjnym zespołów (są one oznaczone jako "wkrótce" w dokumentacji).</span><span class="sxs-lookup"><span data-stu-id="6c4a8-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="6c4a8-107">W takim przypadku lub jeśli pojawia się błąd, taki jak "Nie możemy zaktualizować zasad teraz, ale spróbuj go ponownie później" w centrum administracyjnym programu Microsoft Teams, zaleca się używanie programu PowerShell do tworzenia lub modyfikowania zasad spotkań w programie Teams.</span><span class="sxs-lookup"><span data-stu-id="6c4a8-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="6c4a8-108">Aby uzyskać więcej informacji na temat zasad spotkania, zobacz następujące zasoby:</span><span class="sxs-lookup"><span data-stu-id="6c4a8-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="6c4a8-109">Aby dowiedzieć się więcej o tworzeniu zasad, wprowadzaniu zmian i przypisywaniu użytkowników do zasad, zobacz [Zarządzanie zasadami spotkań w aplikacji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="6c4a8-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="6c4a8-110">Aby wprowadzić zmiany zasad przy użyciu pozsów cmdlet programu PowerShell, zobacz [Omówienie programu Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="6c4a8-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="6c4a8-111">Należy użyć [modułu programu Skype dla firm PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) dla zasad spotkań w zespołach.</span><span class="sxs-lookup"><span data-stu-id="6c4a8-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="6c4a8-112">Aby uzyskać więcej informacji, zapoznaj się z [dokumentacją pozorów cmdlet \*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="6c4a8-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>


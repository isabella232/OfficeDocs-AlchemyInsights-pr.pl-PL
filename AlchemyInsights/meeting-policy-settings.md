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
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627584"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="98df7-102">Zarządzanie zasadami spotkania w programie Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="98df7-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="98df7-103">Zasady spotkania są używane do kontrolowania funkcji, które są dostępne dla uczestników spotkania dla spotkań, które są zaplanowane przez użytkowników w organizacji.</span><span class="sxs-lookup"><span data-stu-id="98df7-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="98df7-104">Niektóre funkcje zasad spotkania mogą nie zostać wdrożone w centrum administracyjnym zespołów jeszcze (są one oznaczone jako "wkrótce" w dokumentacji).</span><span class="sxs-lookup"><span data-stu-id="98df7-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="98df7-105">W tym przypadku lub jeśli otrzymujesz błąd, takich jak "Firma Microsoft nie można zaktualizować zasady teraz, ale spróbuj ponownie później" w centrum administracyjnego programu Teams firmy Microsoftzaleca się używanie programu PowerShell do tworzenia lub modyfikowania zespołów zasad spotkania.</span><span class="sxs-lookup"><span data-stu-id="98df7-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="98df7-106">Aby uzyskać więcej informacji na temat zasad spotkania zobacz następujące zasoby:</span><span class="sxs-lookup"><span data-stu-id="98df7-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="98df7-107">Aby dowiedzieć się więcej na temat tworzenia zasad, wprowadzania zmian i przypisywania użytkowników do zasad, zobacz [Zarządzanie zasadami spotkania w zespołach](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="98df7-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="98df7-108">Aby wprowadzić zmiany zasad za pomocą poleceń cmdlet programu PowerShell, zobacz [Omówienie programu PowerShell zespołów](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="98df7-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="98df7-109">Należy użyć programu [Skype dla modułu Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) dla zespołów spotkań zasad.</span><span class="sxs-lookup"><span data-stu-id="98df7-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="98df7-110">Przejrzyj [dokumentację poleceń cmdlet \*-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) , aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="98df7-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="98df7-111">**Uwaga:** Może potrwać do 24 godzin, aby zmiany zasad zostały uwzględnione dla użytkowników.</span><span class="sxs-lookup"><span data-stu-id="98df7-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="98df7-112">Może nie być możliwe natychmiastowe wprowadzenie zmian w nowo utworzonych zasadach; Poczekaj 4 godziny i spróbuj ponownie zmodyfikować nowo utworzoną zasadę.</span><span class="sxs-lookup"><span data-stu-id="98df7-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="98df7-113">Jeśli nadal występują problemy, Wypróbuj program PowerShell.</span><span class="sxs-lookup"><span data-stu-id="98df7-113">If you're still having problems, try PowerShell.</span></span>  
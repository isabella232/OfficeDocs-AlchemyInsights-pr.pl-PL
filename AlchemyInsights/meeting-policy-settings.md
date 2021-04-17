---
title: Ustawienia zasad spotkania
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825453"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="4f01f-102">Zarządzanie zasadami spotkań w aplikacji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4f01f-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="4f01f-103">**Uwaga: może upłynieć do 24 godzin, aż zmiany zasad zajdą w życie dla użytkowników.**</span><span class="sxs-lookup"><span data-stu-id="4f01f-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="4f01f-104">Być może nie będzie można natychmiast wprowadzić zmian w nowo utworzonych zasadach. Odczekaj 4 godziny i spróbuj ponownie zmodyfikować nowo utworzone zasady.</span><span class="sxs-lookup"><span data-stu-id="4f01f-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="4f01f-105">Zasady spotkań służą do kontrolowania funkcji dostępnych dla uczestników spotkań zaplanowanych przez użytkowników w organizacji.</span><span class="sxs-lookup"><span data-stu-id="4f01f-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="4f01f-106">Niektóre funkcje zasad spotkań mogą nie być jeszcze zaimplementowane w centrum administracyjnym aplikacji Teams (są oznaczone w dokumentacji jako "wkrótce").</span><span class="sxs-lookup"><span data-stu-id="4f01f-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="4f01f-107">W takim przypadku lub w przypadku wystąpienia błędu, takiego jak "Nie możemy w tej chwili zaktualizować zasad, ale spróbujemy ponownie później" w centrum administracyjnym usługi Microsoft Teams, zalecamy używanie programu PowerShell do tworzenia i modyfikowania zasad spotkań aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="4f01f-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="4f01f-108">Aby uzyskać więcej informacji na temat zasad spotkania, zobacz następujące zasoby:</span><span class="sxs-lookup"><span data-stu-id="4f01f-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="4f01f-109">Aby dowiedzieć się więcej o tworzeniu zasad, zmienianiu i przypisywaniu użytkowników do zasad, zobacz [Zarządzanie zasadami spotkań w aplikacji Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="4f01f-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="4f01f-110">Aby wprowadzić zmiany w zasadach przy użyciu poleceń cmdlet programu PowerShell, zobacz [Omówienie programu Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="4f01f-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="4f01f-111">Należy użyć modułu [Skype dla firm PowerShell dla](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) zasad spotkania w aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="4f01f-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="4f01f-112">Przejrzyj [dokumentację polecenia cmdlet \*-CsTeamsMeetingPolicy,](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="4f01f-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>


---
title: Ustawienia zasad spotkania
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704616"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="2436a-102">Zarządzanie zasadami spotkań w aplikacji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2436a-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="2436a-103">**Uwaga: może upłynieć do 24 godzin, aż zmiany zasad zajdą w życie dla użytkowników.**</span><span class="sxs-lookup"><span data-stu-id="2436a-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="2436a-104">Zmiany nowo utworzonych zasad mogą nie być możliwe od razu; Odczekaj 4 godziny i spróbuj ponownie zmodyfikować nowo utworzone zasady.</span><span class="sxs-lookup"><span data-stu-id="2436a-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="2436a-105">Zasady spotkań służą do kontrolowania funkcji dostępnych dla uczestników spotkania w przypadku spotkań zaplanowanych przez użytkowników w organizacji.</span><span class="sxs-lookup"><span data-stu-id="2436a-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="2436a-106">Niektóre funkcje zasad spotkań mogą nie być jeszcze zaimplementowane w centrum administracyjnym aplikacji Teams (w dokumentacji są one oznaczone jako "wkrótce").</span><span class="sxs-lookup"><span data-stu-id="2436a-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="2436a-107">W takim przypadku lub w przypadku wystąpienia błędu, takiego jak "Nie możemy w tej chwili zaktualizować zasad, ale spróbuj ponownie później" w centrum administracyjnym usługi Microsoft Teams, zalecamy używanie programu PowerShell do tworzenia lub modyfikowania zasad spotkań aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="2436a-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="2436a-108">Aby uzyskać więcej informacji na temat zasad spotkań, zobacz następujące zasoby:</span><span class="sxs-lookup"><span data-stu-id="2436a-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="2436a-109">Aby dowiedzieć się, jak tworzyć zasady, wprowadzać zmiany i przypisywać użytkowników do zasad, zobacz Zarządzanie zasadami spotkań w [aplikacji Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="2436a-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="2436a-110">Aby wprowadzić zmiany w zasadach przy użyciu poleceń cmdlet programu PowerShell, zobacz [Omówienie programu Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="2436a-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="2436a-111">Musisz użyć modułu Skype dla [firm PowerShell dla](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) zasad spotkań aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="2436a-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="2436a-112">Aby uzyskać więcej informacji, zapoznaj się z dokumentacją [polecenia cmdlet \*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="2436a-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>


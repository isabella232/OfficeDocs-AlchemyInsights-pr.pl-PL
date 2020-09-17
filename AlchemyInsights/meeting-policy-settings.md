---
title: Ustawienia zasad spotkań
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
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794344"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="0b546-102">Zarządzanie zasadami dotyczącymi spotkań w usłudze Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0b546-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="0b546-103">**Uwaga: wprowadzenie zmian zasad może potrwać do 24 godzin.**</span><span class="sxs-lookup"><span data-stu-id="0b546-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="0b546-104">Użytkownik może nie mieć możliwości natychmiastowego wprowadzenia zmian w nowo utworzonych zasadach. Poczekaj 4 godziny i spróbuj ponownie zmodyfikować nowo utworzone zasady.</span><span class="sxs-lookup"><span data-stu-id="0b546-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="0b546-105">Zasady spotkania służą do kontrolowania funkcji, które są dostępne dla uczestników spotkania w spotkaniach planowanych przez użytkowników w organizacji.</span><span class="sxs-lookup"><span data-stu-id="0b546-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="0b546-106">Niektóre funkcje zasad spotkań mogą nie być zaimplementowane w centrum administracyjnym aplikacji Teams (te elementy są już dostępne w dokumentacji).</span><span class="sxs-lookup"><span data-stu-id="0b546-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="0b546-107">W tym przypadku lub jeśli jest wyświetlany błąd "taki jak nie można teraz zaktualizować zasad, ale spróbuj ponownie później" w centrum administracyjnym usługi Microsoft Teams zalecamy utworzenie lub zmodyfikowanie zasad spotkań zespołów Teams za pomocą programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0b546-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="0b546-108">Aby uzyskać więcej informacji na temat zasad spotkań, zobacz następujące zasoby:</span><span class="sxs-lookup"><span data-stu-id="0b546-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="0b546-109">Aby uzyskać informacje na temat tworzenia zasad, wprowadzania zmian i przypisywania użytkowników do zasad, zobacz [Zarządzanie zasadami dotyczącymi spotkań w aplikacji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="0b546-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="0b546-110">Aby wprowadzić zmiany zasad przy użyciu poleceń cmdlet programu PowerShell, zobacz [Omówienie programu Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="0b546-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="0b546-111">Musisz użyć [modułu programu PowerShell programu Skype dla firm](https://www.microsoft.com/download/details.aspx?id=39366) dla aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="0b546-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="0b546-112">Aby uzyskać więcej informacji, zobacz [dokumentację poleceń cmdlet \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="0b546-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>


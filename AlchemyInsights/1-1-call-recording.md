---
title: Nagrywanie rozmowy 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702100"
---
# <a name="11-call-recording"></a><span data-ttu-id="b6a20-102">Nagrywanie rozmowy 1:1</span><span class="sxs-lookup"><span data-stu-id="b6a20-102">1:1 call recording</span></span>

<span data-ttu-id="b6a20-103">Jeśli przycisk **Rozpocznij nagrywanie** jest wyszarzony w czasie połączenia 1:1, musisz zmienić ustawienia zasad dla użytkownika, na który ma to wpływ.</span><span class="sxs-lookup"><span data-stu-id="b6a20-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="b6a20-104">Aby sprawdzić ustawienie zasad, uruchom narzędzie Diagnostyczne dla użytkownika, u którym ma to wpływ, wpisując **Diag: Teams 1:1 Call Recording above (Rejestrowanie połączeń 1:1).**</span><span class="sxs-lookup"><span data-stu-id="b6a20-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="b6a20-105">Począwszy od 31 maja 2021 r., zaczniemy wymuszanie nowej zasady połączeń usługi Teams *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="b6a20-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="b6a20-106">Przed tą zmianą nagrywanie połączeń 1:1 jest kontrolowane przez zasady spotkań Teams *AllowCloudRecording.*</span><span class="sxs-lookup"><span data-stu-id="b6a20-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="b6a20-107">Ta zmiana została udokumentowana we wpisie w Centrum wiadomości: [(Zaktualizowano) 1:1 Wprowadzenie](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)do zasad nagrywania połączeń.</span><span class="sxs-lookup"><span data-stu-id="b6a20-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="b6a20-108">*AllowCloudRecordingForCalls*   opcję zasad połączeń jest domyślnie **$False** domyślne.</span><span class="sxs-lookup"><span data-stu-id="b6a20-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="b6a20-109">Jeśli wolisz zablokować wszystkim użytkownikom nagrywanie połączeń 1:1, nie musisz nic robić.</span><span class="sxs-lookup"><span data-stu-id="b6a20-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="b6a20-110">Aby włączyć nagrywanie połączeń dla wszystkich użytkowników w połączeniach 1:1, użyj Teams [PowerShell,](/microsoftteams/teams-powershell-install) aby uruchomić następujące polecenie cmdlet:</span><span class="sxs-lookup"><span data-stu-id="b6a20-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="b6a20-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="b6a20-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="b6a20-112">Ewentualnie możesz utworzyć nowe zasady i ustawić ustawienie **-AllowCloudRecordingForCalls** w celu $true i przypisania tych zasad do użytkowników. </span><span class="sxs-lookup"><span data-stu-id="b6a20-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="b6a20-113">Aby uzyskać więcej informacji, zobacz 1:1 Kontrolki zasad nagrywania połączeń [są (prawie!) Tutaj](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="b6a20-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>

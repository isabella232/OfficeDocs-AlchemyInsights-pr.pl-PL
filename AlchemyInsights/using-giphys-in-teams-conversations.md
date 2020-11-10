---
title: Korzystanie z animacjami Giphy w rozmowach zespołów
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982502"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="8188c-102">Korzystanie z animacjami Giphy w rozmowach zespołów</span><span class="sxs-lookup"><span data-stu-id="8188c-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="8188c-103">Animacjami Giphy dostęp w usłudze Teams jest domyślnie włączony.</span><span class="sxs-lookup"><span data-stu-id="8188c-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="8188c-104">Jako administrator możesz kontrolować, czy animacjami Giphy są dostępne dla użytkowników, [ustawiając zasady obsługi wiadomości](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) i upewniając się, że **Korzystanie z animacjami Giphy w konwersacjach** jest **włączone**.</span><span class="sxs-lookup"><span data-stu-id="8188c-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="8188c-105">Jeśli w konwersacjach zespołów pliki GIF nie działają zgodnie z oczekiwaniami, sprawdź, czy:</span><span class="sxs-lookup"><span data-stu-id="8188c-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="8188c-106">[Zasady obsługi wiadomości](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) muszą zezwalać na animacjami Giphy.</span><span class="sxs-lookup"><span data-stu-id="8188c-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="8188c-107">Aby sprawdzić za pomocą poleceń cmdlet programu PowerShell:</span><span class="sxs-lookup"><span data-stu-id="8188c-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="8188c-108">Sprawdź, czy możesz [zarządzać zespołami za pomocą programu PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="8188c-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="8188c-109">Uruchom polecenie programu PowerShell [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i sprawdź, czy **AllowGiphy** jest ustawiona na **wartość true**.</span><span class="sxs-lookup"><span data-stu-id="8188c-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="8188c-110">Jeśli **AllowGiphy** jest ustawiona na **false** , uruchom następujące polecenie programu PowerShell [Set-CsTeamsMessagingPolicy-Identity Global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="8188c-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="8188c-111">W celu umożliwienia dostępu do adresu URL usługi Giphy należy włączyć [opcjonalne środowisko połączone](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .</span><span class="sxs-lookup"><span data-stu-id="8188c-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="8188c-112">Jeśli dla dzierżawy skonfigurowano wiele zasad dotyczących wiadomości programu Teams, możesz określić tożsamość zasad przypisanych do dotkniętego problemem użytkownikowi za pomocą polecenia programu PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Wybierz pozycję TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="8188c-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>

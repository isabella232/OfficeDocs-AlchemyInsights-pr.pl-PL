---
title: Kanał prywatny
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005448"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="ea4db-102">Kanały prywatne w usłudze Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ea4db-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="ea4db-103">Kanały prywatne to nowa funkcja w usłudze Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ea4db-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="ea4db-104">Należy pamiętać, że kanałów prywatnych nie można konwertować ze standardowych kanałów ani odwrotnie.</span><span class="sxs-lookup"><span data-stu-id="ea4db-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="ea4db-105">Aby uzyskać szczegółowe informacje o kanałach prywatnych, takich jak informacje o [tworzeniu kanałów prywatnych i członkostwie](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) oraz [witrynach programu SharePoint kanału prywatnego,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)zobacz [Kanały prywatne w usłudze Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="ea4db-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="ea4db-106">**Uwaga:** Ponieważ konfiguracja przechowywania wiadomości kanału prywatnego nie jest jeszcze obsługiwana, dzierżawcy z włączonymi zasadami przechowywania nie będą domyślnie wstrzymywani kanałów prywatnych.</span><span class="sxs-lookup"><span data-stu-id="ea4db-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="ea4db-107">Kanały prywatne można włączyć w centrum administracyjnym zespołów.</span><span class="sxs-lookup"><span data-stu-id="ea4db-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="ea4db-108">Należy również pamiętać, że podczas przechowywania wiadomości kanału prywatnego nie jest obsługiwany, przechowywanie plików udostępnionych w kanałach prywatnych jest obsługiwane.</span><span class="sxs-lookup"><span data-stu-id="ea4db-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="ea4db-109">**Potrzebujesz nowego właściciela zespołu?**</span><span class="sxs-lookup"><span data-stu-id="ea4db-109">**Need a new team owner?**</span></span>

<span data-ttu-id="ea4db-110">Jeśli twój prywatny właściciel kanału odejdzie, możesz dodać nowego właściciela zespołu za pośrednictwem programu Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="ea4db-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="ea4db-111">Przejdź [tutaj,](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) aby zainstalować program Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="ea4db-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="ea4db-112">Oto polecenie cmdlet, którego potrzebujesz:</span><span class="sxs-lookup"><span data-stu-id="ea4db-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="ea4db-113">Aby uzyskać więcej informacji na temat programu Teams Powershell, zobacz [Omówienie programu Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="ea4db-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>

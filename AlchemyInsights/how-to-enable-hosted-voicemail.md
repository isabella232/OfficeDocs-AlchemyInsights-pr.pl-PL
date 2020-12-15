---
title: Jak włączyć hostowaną pocztę głosową
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679170"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="2bb8d-102">Jak włączyć hostowaną pocztę głosową</span><span class="sxs-lookup"><span data-stu-id="2bb8d-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="2bb8d-103">Aby włączyć pocztę głosową, **HostedVoicemail** musi być ustawiona na $true.</span><span class="sxs-lookup"><span data-stu-id="2bb8d-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="2bb8d-104">Właściwość **HostedVoicemail** użytkownika przy użyciu zdalnego programu POWERSHELL (RPS).</span><span class="sxs-lookup"><span data-stu-id="2bb8d-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="2bb8d-105">Aby uzyskać więcej informacji na temat łączenia się z usługą RPS, zobacz [Omówienie programu Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) , aby uzyskać więcej informacji na temat łączenia się z RPS.</span><span class="sxs-lookup"><span data-stu-id="2bb8d-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="2bb8d-106">Administrator zespołów powinien być zalogowany do zdalnego programu PowerShell dla aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="2bb8d-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="2bb8d-107">Z poziomu monitu programu PowerShell administrator Teams może uruchomić aplikację **Set-csuser user@contoso.com-HostedVoiceMail $true** , gdzie identyfikator URI SIP ma dany użytkownik.</span><span class="sxs-lookup"><span data-stu-id="2bb8d-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="2bb8d-108">Replikowanie zmian zasad może potrwać do 24 godzin.</span><span class="sxs-lookup"><span data-stu-id="2bb8d-108">Changes to policies can take up to 24 hours to replicate.</span></span>
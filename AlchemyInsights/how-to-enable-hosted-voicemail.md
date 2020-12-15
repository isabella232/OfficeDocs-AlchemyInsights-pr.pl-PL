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
# <a name="how-to-enable-hosted-voicemail"></a>Jak włączyć hostowaną pocztę głosową

Aby włączyć pocztę głosową, **HostedVoicemail** musi być ustawiona na $true.

Właściwość **HostedVoicemail** użytkownika przy użyciu zdalnego programu POWERSHELL (RPS).

Aby uzyskać więcej informacji na temat łączenia się z usługą RPS, zobacz [Omówienie programu Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) , aby uzyskać więcej informacji na temat łączenia się z RPS.

1. Administrator zespołów powinien być zalogowany do zdalnego programu PowerShell dla aplikacji Teams.
1. Z poziomu monitu programu PowerShell administrator Teams może uruchomić aplikację **Set-csuser user@contoso.com-HostedVoiceMail $true** , gdzie identyfikator URI SIP ma dany użytkownik.

> [!NOTE]
> Replikowanie zmian zasad może potrwać do 24 godzin.
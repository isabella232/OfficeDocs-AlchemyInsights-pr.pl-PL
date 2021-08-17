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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055564"
---
# <a name="how-to-enable-hosted-voicemail"></a>Jak włączyć hostowaną pocztę głosową

Aby włączyć pocztę głosową, dla poczty **e-mail usługi HostedVoice** musi być $true.

Właściwość **HostedVoicemail** użytkownika przy użyciu zdalnej obsługi programu PowerShell (RESEARCHS).

Aby uzyskać więcej informacji na temat nawiązywania połączeń z tym programem, zobacz Microsoft Teams Omówienie programu [PowerShell,](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) aby uzyskać więcej informacji na temat nawiązywania połączeń z tym programem.

1. Administrator Teams powinien być zalogowany do zdalnej pracy w programie PowerShell dla Teams.
1. W programie PowerShell zostanie wyświetlony monit Teams administrator może uruchomić polecenia **set-csuser user@contoso.com -HostedVoiceMail $true,** gdzie identyfikator uri SIP jest identyfikatorem uri użytkownika.

> [!NOTE]
> Replikowanie zmian w zasadach może potrwać do 24 godzin.
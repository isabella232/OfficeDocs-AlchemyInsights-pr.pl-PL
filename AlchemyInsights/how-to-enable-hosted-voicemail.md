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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318658"
---
# <a name="how-to-enable-hosted-voicemail"></a>Jak włączyć hostowaną pocztę głosową

Aby włączyć pocztę głosową, dla usługi **HostedVoicemail** musi być ustawiona $true.

Właściwość **HostedVoicemail** użytkownika przy użyciu zdalnej obsługi programu PowerShell (RESEARCHS).

Aby uzyskać więcej informacji na temat nawiązywania połączeń z tym programem, zobacz Microsoft Teams Omówienie programu [PowerShell,](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) aby uzyskać więcej informacji na temat nawiązywania połączeń z tym programem.

1. Administrator Teams powinien być zalogowany do zdalnej pracy w programie PowerShell dla Teams.
1. W programie PowerShell zostanie wyświetlony monit Teams administrator programu może uruchomić usługę **set-csuser user@contoso.com-HostedVoiceMail $true,** gdzie identyfikator uri SIP jest wyświetlany dla danych użytkownika.

**Uwaga:** Replikowanie zmian w zasadach może potrwać do 24 godzin.
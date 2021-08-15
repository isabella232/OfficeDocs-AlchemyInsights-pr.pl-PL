---
title: Włączanie technologii NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023532"
---
# <a name="turn-on-ndi-technology"></a>Włączanie technologii NDI

Technologia NDI wymaga, aby użytkownik włączył dwa kroki:

1. Administrator dzierżawy musi włączyć właściwość "AllowNDIStreaming" w ujmowaniu w usługę CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Po wpełnieniu tej zmiany użytkownik końcowy musi włączyć technologię NDI® dla swojego klienta z poziomu strony **Ustawienia > uprawnienia.**

Aby uzyskać więcej informacji, zobacz [Korzystanie z technologii NDI w Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)

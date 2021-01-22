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
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935134"
---
# <a name="turn-on-ndi-technology"></a>Włączanie technologii NDI

Technologia NDI wymaga, aby użytkownik włączył dwie czynności:

1. Administrator dzierżawy musi włączyć właściwość "AllowNDIStreaming" w u administratora usługi CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Po wpełnieniu tej zmiany użytkownik końcowy musi włączyć technologię NDI® dla swojego konkretnego klienta z poziomu ustawień **> uprawnień.**

Aby uzyskać więcej informacji, zobacz [Korzystanie z technologii NDI w aplikacji Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)

---
title: Ciąg agenta użytkownika programu Microsoft Edge (pulpit)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679338"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a>Ciąg agenta użytkownika programu Microsoft Edge (pulpit)

Za pomocą ciągów agenta użytkownika (UA) można wykryć, która wersja konkretnej przeglądarki jest używana w pewnym systemie operacyjnym. Podobnie jak w przypadku innych przeglądarek, program Microsoft Edge uwzględnia te informacje w nagłówku HTTP "User-Agent", ilekroć wysyła żądanie do witryny. Dostęp do informacji w przeglądarce można uzyskać również za pośrednictwem języka JavaScript, wykonując zapytanie dotyczące wartości "Navigator. userAgent".

Zalecamy, aby deweloperzy korzystający z sieci Web używali wykrywania funkcji, ilekroć tylko jest to możliwe, aby zwiększyć łatwość obsługi kodu, zmniejszyć wrażliwość kodu i wyeliminować ryzyko złamania kodu w przypadku przyszłych aktualizacji ciągów UA.

Aby uzyskać więcej informacji, zobacz [ciąg agenta użytkownika programu Microsoft Edge (komputer stacjonarny)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).
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
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="2f034-102">Ciąg agenta użytkownika programu Microsoft Edge (pulpit)</span><span class="sxs-lookup"><span data-stu-id="2f034-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="2f034-103">Za pomocą ciągów agenta użytkownika (UA) można wykryć, która wersja konkretnej przeglądarki jest używana w pewnym systemie operacyjnym.</span><span class="sxs-lookup"><span data-stu-id="2f034-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="2f034-104">Podobnie jak w przypadku innych przeglądarek, program Microsoft Edge uwzględnia te informacje w nagłówku HTTP "User-Agent", ilekroć wysyła żądanie do witryny.</span><span class="sxs-lookup"><span data-stu-id="2f034-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="2f034-105">Dostęp do informacji w przeglądarce można uzyskać również za pośrednictwem języka JavaScript, wykonując zapytanie dotyczące wartości "Navigator. userAgent".</span><span class="sxs-lookup"><span data-stu-id="2f034-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="2f034-106">Zalecamy, aby deweloperzy korzystający z sieci Web używali wykrywania funkcji, ilekroć tylko jest to możliwe, aby zwiększyć łatwość obsługi kodu, zmniejszyć wrażliwość kodu i wyeliminować ryzyko złamania kodu w przypadku przyszłych aktualizacji ciągów UA.</span><span class="sxs-lookup"><span data-stu-id="2f034-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="2f034-107">Aby uzyskać więcej informacji, zobacz [ciąg agenta użytkownika programu Microsoft Edge (komputer stacjonarny)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="2f034-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>
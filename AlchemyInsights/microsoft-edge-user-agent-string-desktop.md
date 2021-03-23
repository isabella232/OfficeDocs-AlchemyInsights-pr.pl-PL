---
title: Ciągi agentów użytkownika programu Microsoft Edge (wersja komputerowa)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8221"
- "9004596"
ms.openlocfilehash: 42c39f5661f57c7b57fa471f9c204e5c27f2f214
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037296"
---
# <a name="microsoft-edge-user-agent-strings-desktop"></a><span data-ttu-id="d222f-102">Ciągi agentów użytkownika programu Microsoft Edge (wersja komputerowa)</span><span class="sxs-lookup"><span data-stu-id="d222f-102">Microsoft Edge user agent strings (Desktop)</span></span>

<span data-ttu-id="d222f-103">Ciągi agenta użytkownika (UA) mogą służyć do wykrywania wersji określonej przeglądarki używanej w określonym systemie operacyjnym.</span><span class="sxs-lookup"><span data-stu-id="d222f-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="d222f-104">Podobnie jak w innych przeglądarkach przeglądarka Microsoft Edge zawsze, gdy poprosi o to witrynę, będzie ona uwzględniać te informacje w nagłówku HTTP "User-Agent".</span><span class="sxs-lookup"><span data-stu-id="d222f-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="d222f-105">Można też uzyskać do niego dostęp za pośrednictwem języka JavaScript, kwerendując wartość ciągu "navigator.userAgent".</span><span class="sxs-lookup"><span data-stu-id="d222f-105">It can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="d222f-106">Zalecamy, aby deweloperzy sieci Web zawsze, gdy to możliwe, korzystali z wykrywania funkcji, aby poprawić konserwację kodu, zmniejszyć niestabilność kodu i wyeliminować ryzyko łamania kodu w przypadku przyszłych aktualizacji ciągów UA.</span><span class="sxs-lookup"><span data-stu-id="d222f-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="d222f-107">Aby uzyskać więcej informacji, zobacz [Ciąg agenta użytkownika programu Microsoft Edge (wersja komputerowa).](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)</span><span class="sxs-lookup"><span data-stu-id="d222f-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>


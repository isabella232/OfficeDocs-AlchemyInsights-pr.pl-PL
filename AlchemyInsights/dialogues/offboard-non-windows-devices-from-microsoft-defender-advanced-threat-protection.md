---
title: Urządzenia typu Offboard, które nie są urządzeniami z systemem Windows, od usługi Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695155"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="e2aa5-102">Urządzenia typu Offboard, które nie są urządzeniami z systemem Windows, od usługi Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="e2aa5-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="e2aa5-103">W tym celu wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="e2aa5-103">Here's how:</span></span>

1. <span data-ttu-id="e2aa5-104">Postępuj zgodnie z dokumentacją innej firmy w celu odłączenia rozwiązania innej firmy od programu Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="e2aa5-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="e2aa5-105">W dzierżawie usługi Azure Active Directory usuń uprawnienia do rozwiązania innej firmy:</span><span class="sxs-lookup"><span data-stu-id="e2aa5-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="e2aa5-106">Zaloguj się do [portalu Azure Portal.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="e2aa5-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="e2aa5-107">Wybierz **pozycję Wszystkie usługi** Azure Active  >  **Directory** Enterprise  >  **Applications.**</span><span class="sxs-lookup"><span data-stu-id="e2aa5-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="e2aa5-108">Wybierz aplikację, która ma być wyniesiena.</span><span class="sxs-lookup"><span data-stu-id="e2aa5-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="e2aa5-109">Wybierz **pozycję Usuń.**</span><span class="sxs-lookup"><span data-stu-id="e2aa5-109">Select **Delete**.</span></span>

<span data-ttu-id="e2aa5-110">Aby dowiedzieć się więcej, [zobacz "Urządzenia przenośne typu Offboard", na których nie ma systemu Windows.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="e2aa5-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>

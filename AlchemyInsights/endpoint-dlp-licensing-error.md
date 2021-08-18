---
title: Błąd licencjonowania usługi DLP punktu końcowego
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090160"
---
# <a name="endpoint-dlp-licensing-error"></a>Błąd licencjonowania usługi DLP punktu końcowego

Jeśli podczas próby skonfigurowania ochrony przed wartością DLP punktu końcowego występuje następujący błąd:

`Your organization is missing the licenses required to manage these devices`.

Upewnij się, że masz jedną z następujących subskrypcji lub dodatków:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 zgodności
- Microsoft 365 A5 zgodności
- Microsoft 365 E5 i zarządzanie informacjami
- Microsoft 365 A5 i zarządzanie informacjami

> [!NOTE]
> Nie będzie to działać w przypadku kombinacji licencji, takiej jak: Win E5 + O365 E5 + EMS E5. Aby skonfigurować tę funkcję, musisz mieć licencję wyłącznie M365 E5.

Aby uzyskać więcej informacji na temat licencjonowania ochrony przed dlp punktami końcowymi, zobacz [Licencjonowanie ochrony przed dlp punktami końcowymi.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)

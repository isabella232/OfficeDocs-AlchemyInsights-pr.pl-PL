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
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322141"
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

**Uwaga:** Nie będzie to działać w przypadku kombinacji licencji, takiej jak: Win E5 + O365 E5 + EMS E5. Aby skonfigurować tę funkcję, musisz mieć licencję wyłącznie M365 E5.

Aby uzyskać więcej informacji na temat licencjonowania ochrony przed dlp punktami końcowymi, zobacz [Licencjonowanie ochrony przed dlp punktami końcowymi.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)

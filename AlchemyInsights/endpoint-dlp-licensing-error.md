---
title: Błąd licencjonowania DLP punktu końcowego
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
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564864"
---
# <a name="endpoint-dlp-licensing-error"></a>Błąd licencjonowania DLP punktu końcowego

Jeśli podczas próby skonfigurowania funkcji DLP punktu końcowego zostanie wyświetlony następujący komunikat o błędzie:

`Your organization is missing the licenses required to manage these devices`.

Upewnij się, że masz jednej z następujących subskrypcji lub dodatków:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Zgodność z programem Microsoft 365 E5
- Zgodność z programem Microsoft 365 A5
- Microsoft 365 E5 Information Protection i zarządzanie
- Microsoft 365 A5 Information Protection and ładu

> [!NOTE]
> Nie będzie to działać w przypadku kombinacji licencji, takich jak: win E5 + O365 E5 + EMS E5. Aby skonfigurować tę funkcję, musisz mieć czystą M365 E5.

Aby uzyskać więcej informacji dotyczących licencjonowania DLP punktu końcowego, zobacz [Licencjonowanie DLP punktu końcowego.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)

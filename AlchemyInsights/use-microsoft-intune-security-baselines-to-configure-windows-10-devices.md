---
title: Konfigurowanie urządzeń z systemem Windows 10 przy użyciu planu bazowego zabezpieczeń usługi Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696377"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Konfigurowanie urządzeń z systemem Windows 10 przy użyciu planu bazowego zabezpieczeń usługi Microsoft Intune

Plan bazowy zabezpieczeń usługi Intune pomaga chronić użytkowników i urządzenia. Plan bazowy zabezpieczeń to wstępnie skonfigurowane grupy systemu Windows służące do stosowania znanej grupy ustawień i wartości domyślnych zalecanych przez odpowiednie zespoły ds. zabezpieczeń. Tworząc profil planu bazowego zabezpieczeń w usłudze Intune, tworzysz szablon składający się z wielu profilów konfiguracji urządzenia.

Podczas wdrażania planu bazowego zabezpieczeń dla grup użytkowników lub urządzeń ustawienia są stosowane do urządzeń uruchamianych w systemie Windows 10 lub nowszym. Na przykład plan bazowy zabezpieczeń zarządzania urządzeniami przenośnymi firmy Microsoft (MDM) automatycznie (1) włącza funkcję BitLocker dla dysków wymiennych, (2) wymaga hasła do odblokowania urządzenia, a (3) wyłącza uwierzytelnianie podstawowe. Jeśli wartość domyślna nie działa w Twoim środowisku, możesz dostosować plan bazowy, aby zastosować potrzebne ustawienia.

Plan bazowy zabezpieczeń pomaga również w ustanawianiu end-to-end bezpiecznego przepływu pracy na platformy Microsoft 365. Oto niektóre z zalet tej funkcji:
- Plan bazowy zabezpieczeń zawiera najlepsze rozwiązania i zalecenia dotyczące ustawień mających wpływ na bezpieczeństwo. Ponieważ usługa Intune współpracuje z zespołem zabezpieczeń systemu Windows, który tworzy plan bazowy dla zasad grupy, te zalecenia są oparte na pełnych wskazówkach i obszernym doświadczeniu.
- Jeśli nie masz pewności, od czego zacząć, nie wiesz, od czego zacząć, plan bazowy zabezpieczeń pomoże Ci szybko utworzyć i wdrożyć bezpieczny profil.
- Jeśli obecnie korzystasz z zasad grupy, migracja do intune w celu zarządzania jest znacznie łatwiejsza dzięki planom bazowym zabezpieczeń, ponieważ te linie bazowe zabezpieczeń są wbudowane w usługę Intune i obejmują najnowodniej dostępne funkcje zarządzania.

Aby uzyskać więcej informacji, zobacz [plan bazowy zabezpieczeń systemu Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) i zarządzanie urządzeniami [przenośnymi.](https://docs.microsoft.com/windows/client-management/mdm/)
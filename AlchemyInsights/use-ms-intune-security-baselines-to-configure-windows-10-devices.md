---
title: Konfigurowanie Microsoft Intune przy użyciu podstawowych planu bazowego Windows 10 zabezpieczeń
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104354"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfigurowanie Microsoft Intune przy użyciu podstawowych planu bazowego Windows 10 zabezpieczeń

Linie bazowe zabezpieczeń usługi Intune pomagają chronić użytkowników i urządzenia. Linie bazowe zabezpieczeń Windows wstępnie skonfigurowane grupy ustawień używane do stosowania znanej grupy ustawień i wartości domyślnych zalecanych przez odpowiednie zespoły zabezpieczeń. Tworząc profil planu bazowego zabezpieczeń w usłudze Intune, tworzysz szablon składający się z wielu profilów konfiguracji urządzeń.

Podczas wdrażania planu bazowego zabezpieczeń w grupach użytkowników lub urządzeń ustawienia są stosowane do urządzeń uruchamianych Windows 10 lub nowszym. Na przykład funkcja Plan bazowy zabezpieczeń MDM automatycznie (1) włącza funkcję BitLocker dla dysków wymiennych, (2) wymaga hasła do odblokowania urządzenia, a (3) wyłącza uwierzytelnianie podstawowe. Jeśli wartość domyślna nie działa w Twoim środowisku, dostosuj plan bazowy, aby zastosować potrzebne ustawienia.

Linie bazowe zabezpieczeń ułatwiają również utworzenie bezpiecznego, bezpiecznego przepływu pracy w Microsoft 365. Oto kilka korzyści z tego:

- Plan bazowy zabezpieczeń zawiera najlepsze rozwiązania i zalecenia dotyczące ustawień wpływających na bezpieczeństwo. Ponieważ usługa Intune współpracuje z zespołem zabezpieczeń Windows, który tworzy linie bazowe zasad grupy, zalecenia te są oparte na pełnych wskazówkach i obszernym doświadczeniu.
- Jeśli nie masz pewności, od czego zacząć, to plan bazowy zabezpieczeń pomoże Ci szybko utworzyć i wdrożyć bezpieczny profil, jeśli nie masz pewności, od czego zacząć.
- Jeśli obecnie korzystasz z zasad grupy, migracja do usługi Intune w celu zarządzania jest znacznie łatwiejsza dzięki planom bazowym zabezpieczeń, ponieważ są one wbudowane w usługę Intune i zawierają najnowe możliwości zarządzania.

Aby dowiedzieć się więcej, [zobacz Windows planu bazowego zabezpieczeń](https://go.microsoft.com/fwlink/?linkid=2141503) i Zarządzanie urządzeniami [przenośnymi.](https://go.microsoft.com/fwlink/?linkid=2141701)
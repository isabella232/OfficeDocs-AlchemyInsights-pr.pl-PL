---
title: Konfigurowanie Microsoft Intune przy użyciu podstawowych planu bazowego Windows 10 zabezpieczeń
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793894"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfigurowanie Microsoft Intune przy użyciu podstawowych planu bazowego Windows 10 zabezpieczeń

Linie bazowe zabezpieczeń usługi Intune pomagają chronić użytkowników i urządzenia. Plan bazowy zabezpieczeń Windows wstępnie skonfigurowane grupy używane do stosowania znanej grupy ustawień i wartości domyślnych zalecanych przez odpowiednie zespoły zabezpieczeń. Tworząc profil planu bazowego zabezpieczeń w usłudze Intune, tworzysz szablon składający się z wielu profilów konfiguracji urządzeń.

Podczas wdrażania planu bazowego zabezpieczeń w grupach użytkowników lub urządzeń ustawienia są stosowane do urządzeń uruchamianych Windows 10 lub nowszym. Na przykład plan bazowy zabezpieczeń zarządzania urządzeniami przenośnymi firmy Microsoft automatycznie włącza funkcję funkcja BitLocker dla dysków wymiennych, wymaga hasła do odblokowania urządzenia i wyłącza uwierzytelnianie podstawowe. Jeśli wartość domyślna nie działa w Twoim środowisku, możesz dostosować plan bazowy, aby zastosować potrzebne ustawienia.

Linie bazowe zabezpieczeń ułatwiają również utworzenie bezpiecznego, bezpiecznego przepływu pracy w Microsoft 365. Plan bazowy zabezpieczeń zawiera najlepsze rozwiązania i zalecenia dotyczące ustawień wpływających na bezpieczeństwo. Usługa Intune współpracuje z zespołem zabezpieczeń Windows, który tworzy linie bazowe zasad grupy, więc te zalecenia są oparte na pełnych wskazówkach i obszernym doświadczeniu.

Jeśli nie masz pewności, od czego zacząć, to plan bazowy zabezpieczeń pomoże Ci szybko utworzyć i wdrożyć bezpieczny profil, jeśli nie masz pewności, od czego zacząć. Jeśli obecnie korzystasz z zasad grupy, migracja do usługi Intune do celów zarządzania jest znacznie łatwiejsza dzięki planom bazowym zabezpieczeń, ponieważ są one wbudowane w usługę Intune i zawierają najnowe możliwości zarządzania.

Aby dowiedzieć się więcej, [zobacz Windows planu bazowego zabezpieczeń](/windows/security/threat-protection/windows-security-baselines) i Zarządzanie urządzeniami [przenośnymi.](/windows/client-management/mdm/)


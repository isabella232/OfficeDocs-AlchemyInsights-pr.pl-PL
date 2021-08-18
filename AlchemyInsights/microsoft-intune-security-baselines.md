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
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331995"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfigurowanie Microsoft Intune przy użyciu podstawowych planu bazowego Windows 10 zabezpieczeń

Linie bazowe zabezpieczeń usługi Intune pomagają chronić użytkowników i urządzenia. Plan bazowy zabezpieczeń Windows wstępnie skonfigurowane grupy używane do stosowania znanej grupy ustawień i wartości domyślnych zalecanych przez odpowiednie zespoły zabezpieczeń. Tworząc profil planu bazowego zabezpieczeń w usłudze Intune, tworzysz szablon składający się z wielu profilów konfiguracji urządzeń.

Podczas wdrażania planu bazowego zabezpieczeń w grupach użytkowników lub urządzeń ustawienia są stosowane do urządzeń uruchamianych Windows 10 lub nowszym. Na przykład plan bazowy zabezpieczeń zarządzania urządzeniami przenośnymi (MDM) firmy Microsoft automatycznie włącza funkcję BitLocker dla dysków wymiennych, wymaga hasła do odblokowania urządzenia i wyłącza uwierzytelnianie podstawowe. Jeśli wartość domyślna nie działa w Twoim środowisku, możesz dostosować plan bazowy, aby zastosować potrzebne ustawienia.

Linie bazowe zabezpieczeń ułatwiają również utworzenie bezpiecznego przepływu pracy w programie Microsoft 365. Plan bazowy zabezpieczeń zawiera najlepsze rozwiązania i zalecenia dotyczące ustawień wpływających na bezpieczeństwo. Usługa Intune współpracuje z zespołem zabezpieczeń Windows, który tworzy linie bazowe zasad grupy, więc zalecenia te są oparte na pełnych wskazówkach i obszernym doświadczeniu.

Jeśli nie masz pewności, od czego zacząć, to nowe konto w usłudze Intune pomoże Ci szybko utworzyć i wdrożyć bezpieczny profil. Jeśli obecnie korzystasz z zasad grupy, migracja do usługi Intune do celów zarządzania jest znacznie łatwiejsza dzięki planom bazowym zabezpieczeń, ponieważ są one wbudowane w usługę Intune i zawierają najnowe możliwości zarządzania.

Aby dowiedzieć się więcej, [zobacz Windows planu bazowego zabezpieczeń](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) i Zarządzanie urządzeniami [przenośnymi.](https://docs.microsoft.com/windows/client-management/mdm/)


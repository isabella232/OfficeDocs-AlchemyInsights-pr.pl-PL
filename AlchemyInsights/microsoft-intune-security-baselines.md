---
title: Konfigurowanie Microsoft Intune zabezpieczeń przy użyciu Windows 10 bazowych
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
ms.openlocfilehash: f77fdbb315db8317a6a1374f05489a7f5a0bedcec484dc9ac53a473098583949
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886642"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfigurowanie Microsoft Intune zabezpieczeń przy użyciu Windows 10 bazowych

Linie bazowe zabezpieczeń usługi Intune pomagają chronić użytkowników i urządzenia. Linie bazowe zabezpieczeń Windows wstępnie skonfigurowane grupy używane do stosowania znanej grupy ustawień i wartości domyślnych zalecanych przez odpowiednie zespoły zabezpieczeń. Tworząc profil planu bazowego zabezpieczeń w usłudze Intune, tworzysz szablon składający się z wielu profilów konfiguracji urządzeń.

Podczas wdrażania planu bazowego zabezpieczeń w grupach użytkowników lub urządzeń ustawienia są stosowane do urządzeń uruchamianych Windows 10 lub nowszym. Na przykład plan bazowy zabezpieczeń zarządzania urządzeniami przenośnymi (MDM) firmy Microsoft automatycznie włącza funkcję BitLocker dla dysków wymiennych, wymaga hasła do odblokowania urządzenia i wyłącza uwierzytelnianie podstawowe. Jeśli wartość domyślna nie działa w Twoim środowisku, możesz dostosować plan bazowy, aby zastosować potrzebne ustawienia.

Linie bazowe zabezpieczeń ułatwiają również utworzenie bezpiecznego przepływu pracy w programie Microsoft 365. Plan bazowy zabezpieczeń zawiera najlepsze rozwiązania i zalecenia dotyczące ustawień wpływających na bezpieczeństwo. Usługa Intune współpracuje z zespołem zabezpieczeń Windows, który tworzy linie bazowe zasad grupy, więc te zalecenia są oparte na pełnych wskazówkach i obszernym środowisku.

Jeśli nie masz pewności, od czego zacząć, to nowe konto w usłudze Intune pomoże Ci szybko utworzyć i wdrożyć bezpieczny profil. Jeśli obecnie korzystasz z zasad grupy, migracja do usługi Intune do celów zarządzania jest znacznie łatwiejsza dzięki planom bazowym zabezpieczeń, ponieważ są one wbudowane w usługę Intune i zawierają najnowe możliwości zarządzania.

Aby dowiedzieć się więcej, [zobacz Windows planu bazowego zabezpieczeń](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) i Zarządzanie urządzeniami [przenośnymi.](https://docs.microsoft.com/windows/client-management/mdm/)


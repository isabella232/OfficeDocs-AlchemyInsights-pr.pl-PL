---
title: Konfigurowanie urządzeń z systemem Windows 10 przy użyciu planów bazowych zabezpieczeń usługi Microsoft Intune
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
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573535"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfigurowanie urządzeń z systemem Windows 10 przy użyciu planów bazowych zabezpieczeń usługi Microsoft Intune

Plany bazowe dotyczące zabezpieczeń usługi Intune pomagają chronić użytkowników i urządzenia. Linie bazowe zabezpieczeń to wstępnie skonfigurowane grupy ustawień systemu Windows, używane do stosowania znanej grupy ustawień i wartości domyślnych zalecanych przez odpowiednie zespoły zabezpieczeń. Tworząc profil planu bazowego zabezpieczeń w usłudze Intune, można utworzyć szablon składający się z wielu profilów konfiguracji urządzeń.

Podczas wdrażania planów bazowych zabezpieczeń do grup użytkowników lub urządzeń ustawienia są stosowane do urządzeń z systemem Windows 10 lub nowszym. Na przykład linia bazowa zabezpieczeń oprogramowania MDM automatycznie (1) włącza funkcję BitLocker dla dysków wymiennych, (2) wymaga hasła do odblokowania urządzenia, a (3) wyłącza uwierzytelnianie podstawowe. Jeśli wartość domyślna nie działa w danym środowisku, Dostosuj plan bazowy, aby zastosować potrzebne ustawienia.

Plany bazowe zabezpieczeń ułatwiają również ustanowienie bezpiecznego przepływu pracy w programie Microsoft 365. Poniżej przedstawiono niektóre zalety tego rozwiązania:

- Plan zabezpieczeń zawiera najważniejsze wskazówki i zalecenia dotyczące ustawień wpływających na bezpieczeństwo. Ponieważ partnerzy usługi Intune z zespołem zabezpieczeń systemu Windows, który tworzy plany bazowe dla zasad grupy, te zalecenia są oparte na stałych wskazówkach i rozległych wrażeniach.
- Jeśli nie znasz usługi Intune i nie wiesz, gdzie zacząć, punkty odniesienia w zabezpieczeniach ułatwią szybkie tworzenie i wdrażanie bezpiecznego profilu.
- Jeśli obecnie korzystasz z zasad grupy, przeprowadzenie migracji do usługi Intune w celu zarządzania jest znacznie łatwiejsze w przypadku planów bezpieczeństwa, ponieważ są one wbudowane w usługę Intune i obejmują funkcje obcinania w celu zarządzania.

Aby dowiedzieć się więcej, zobacz [Plan bazowy zabezpieczeń systemu Windows](https://go.microsoft.com/fwlink/?linkid=2141503) i [Zarządzanie urządzeniami przenośnymi](https://go.microsoft.com/fwlink/?linkid=2141701).
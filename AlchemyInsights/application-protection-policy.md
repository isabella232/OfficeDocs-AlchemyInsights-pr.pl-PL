---
title: Zasady ochrony aplikacji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423965"
---
# <a name="application-protection-policy"></a>Zasady ochrony aplikacji

Jeśli jesteś nowym użytkownikiem zasad ochrony aplikacji (APP), zapoznaj się z [omówieniem zasad ochrony aplikacji](https://docs.microsoft.com/intune/apps/app-protection-policy).

Aby rozpocząć korzystanie z aplikacji, zobacz [Jak tworzyć i przypisywać zasady ochrony aplikacji](https://docs.microsoft.com/intune/app-protection-policies).

Wymagania dotyczące zasad ochrony aplikacji:

- Użytkownik ma licencję usługi Intune lub EMS.
- Użytkownik należy do grupy, której dotyczy zasady ochrony aplikacji.
- Tylko jeden użytkownik firmowy jest zalogowany do chronionych aplikacji na urządzeniu.
- Aplikacja zaimplementowała [sdk usługi Intune](https://docs.microsoft.com/intune/app-sdk-get-started). Aby uzyskać listę aplikacji obsługujących pakiet SDK, zobacz [Aplikacje chronione usługi Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Zasady mają zastosowanie po tym, jak użytkownik, który spełnia powyższe wymagania, zaloguje się do aplikacji obsługującej sdk usługi Intune. Najprostszym sposobem określenia, czy zasada jest stosowana, jest wymaganie, aby użytkownik ustawił pinezkę w zasadach. 

Aby uzyskać więcej informacji, zobacz:

[Często zadawane pytania dotyczące rozwiązywania problemów z aplikacją/mam](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Jak sprawdzić poprawność konfiguracji zasad ochrony aplikacji](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Opis harmonogramu dostarczania zasad ochrony aplikacji](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Jak monitorować zasady ochrony aplikacji](https://docs.microsoft.com/intune/app-protection-policies-monitor)
---
title: Menedżer programu EndPoint — linie bazowe zabezpieczeń
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421086"
---
# <a name="endpoint-manager---security-baselines"></a>Menedżer programu EndPoint — linie bazowe zabezpieczeń

Linie bazowe zabezpieczeń to wstępnie skonfigurowane grupy ustawień systemu Windows, które ułatwiają stosowanie ustawień zabezpieczeń zalecanych przez odpowiednie zespoły ds. zabezpieczeń. Te linie bazowe można dostosować, aby dostarczyć tylko żądane ustawienia i wartości. Aby uzyskać więcej informacji o planach bazowych zabezpieczeń, zobacz Konfigurowanie urządzeń z systemem [Windows 10](https://docs.microsoft.com/mem/intune/protect/security-baselines)w usłudze Intune przy użyciu planu bazowego zabezpieczeń.

Obecnie istnieją linie bazowe dla tych produktów:

- Ustawienia zabezpieczeń usługi Windows MDM
- Program Microsoft Defender dla zabezpieczeń programu EndPoint
- Microsoft Edge

Poszczególne linie bazowe są okresowo aktualizowane i zwalniane w wersjach przyrostowych. Każda wersja dodaje i lub usuwa ustawienia z poprzedniej wersji, aby zapewnić, że plan bazowy spełnia bieżące wytyczne. Konsola planu bazowego zabezpieczeń w zabezpieczeniach punktu końcowego umożliwia porównanie różnych wersji przez wprowadzenie zmian w poszczególnych wersjach.

Aby uzyskać wskazówki dotyczące najbardziej efektywnej zmiany wersji planu bazowego, zobacz Zarządzanie profilami planu bazowego zabezpieczeń w [usłudze Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

Po wdrożeniu planu bazowego zabezpieczeń możesz monitorować stan wdrożenia i przeglądać ustawienia w zależności od urządzenia.

**Uwaga:** Dane raportowania dla planu bazowego mogą być wyświetlane w ciągu 24 godzin od wdrożenie wstępne do urządzenia i do 6 godzin na dodatkowe aktualizacje. 

Najczęstszą przyczyną nie zastosowania ustawienia planu bazowego jest to, że to samo ustawienie jest używane w innym profilu. Ten scenariusz można zbadać dla określonego urządzenia, wybierając je w węźle Stan urządzenia profilu planu bazowego zabezpieczeń. Aby uzyskać szczegółowe informacje, zobacz [Rozwiązywanie konfliktów dotyczących planu bazowego zabezpieczeń.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)
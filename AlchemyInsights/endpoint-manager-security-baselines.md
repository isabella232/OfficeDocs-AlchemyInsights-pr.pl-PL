---
title: Endpoint Manager — Plany bazowe zabezpieczeń
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
- "10064"
- "9003771"
ms.openlocfilehash: c13bc161b19a5fef1352beb28bdcc20110111a9a61a47433d82e1e69aff7f88d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978171"
---
# <a name="endpoint-manager---security-baselines"></a>Endpoint Manager — Plany bazowe zabezpieczeń

Plany bazowe zabezpieczeń to wstępnie skonfigurowane grupy ustawień systemu Windows, które ułatwiają stosowanie ustawień zabezpieczeń zalecanych przez odpowiednie zespoły ds. zabezpieczeń. Te plany bazowe można dostosować tak, aby zawierały tylko wymagane ustawienia i wartości. Aby uzyskać więcej informacji o planach bazowych zabezpieczeń, zobacz [Używanie planów bazowych zabezpieczeń do konfigurowania urządzeń z systemem Windows 10 w usłudze Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Obecnie są dostępne plany bazowe dla tych produktów:

- Ustawienia zabezpieczeń funkcji zarządzania urządzeniami przenośnymi z systemem Windows
- Zabezpieczenia usługi Ochrona punktu końcowego w usłudze Microsoft Defender
- Microsoft Edge

Wszystkie plany bazowe są okresowo aktualizowane i wydawane w wersjach przyrostowych. Każda wersja dodaje ustawienia do poprzedniej wersji lub usuwa je z niej, aby zapewnić, że plan bazowy spełnia bieżące wytyczne. Konsola planów bazowych zabezpieczeń w zabezpieczeniach punktów końcowych umożliwia porównanie różnych wersji przez uwidocznienie zmian wprowadzanych w poszczególnych wersjach.

Aby uzyskać wskazówki dotyczące najskuteczniejszego zmieniania wersji wdrożonego planu bazowego, zobacz [Zarządzanie profilami planu bazowego zabezpieczeń w usłudze Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Po wdrożeniu planu bazowego zabezpieczeń możesz monitorować stan wdrożenia i przeglądać ustawienia na poszczególnych urządzeniach.

**Uwaga:** Zanim dane raportowania dla planów bazowych będą widoczne, od momentu wdrożenia wstępnego na urządzeniu może upłynąć do 24 godzin, a w przypadku kolejnych aktualizacji do 6 godzin. 

Najczęstszą przyczyną niezastosowania ustawienia planu bazowego jest to, że to samo ustawienie jest używane w innym profilu. Ten scenariusz można zbadać dla konkretnego urządzenia, wybierając to urządzenie w węźle Stan urządzenia profilu planu bazowego zabezpieczeń. Aby uzyskać szczegółowe informacje, zobacz [Rozwiązywanie konfliktów dotyczących planów bazowych zabezpieczeń](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).
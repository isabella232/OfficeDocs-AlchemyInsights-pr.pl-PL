---
title: 'AIP: Zasady nie zachowujące się zgodnie z oczekiwaniami'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493163"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Zasady nie zachowujące się zgodnie z oczekiwaniami

Usługa Azure Information Protection: Zasady nie zachowujące się zgodnie z oczekiwaniami, zobacz następujące wskazówki dotyczące zalecanych wskazówek dotyczących różnych problemów z zasadami:

1. Jeśli masz problemy z oznaczeniami wizualnymi, zapoznaj się z [oceną, kiedy stosowane są oznaczenia wizualne.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Jeśli masz problemy z automatycznym etykietowaniem, zapoznaj się z [instrukcjami konfigurowania warunków automatycznej i zalecanej klasyfikacji dla usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i czego szukają [typy poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
3. Jeśli masz problemy z ochroną natywną/pfile, zapoznaj się z [konfiguracją interfejsu API plików](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Sprawdź, czy używasz zasad o określonym zakresie, które nie są poprawnie skonfigurowane: [Jak skonfigurować zasady usługi Azure Information Protection dla określonych użytkowników przy użyciu zasad o określonym zakresie.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Jeśli automatyczne etykietowanie nie działa w programie Outlook podczas dołączania dokumentu z etykietą, sprawdź, czy drmencryptProperty nie jest zdefiniowany w sposób opisany w tym miejscu: [Ustawienia rejestru IRM dla zabezpieczeń](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Jeśli nadal występują problemy, zbieraj dzienniki klientów usługi Azure Information Protection i dołączaj eksportowane dzienniki do tego biletu.

1. Otwórz dokument pakietu Office lub utwórz nową wiadomość e-mail w programie Outlook.
2. Kliknij pozycję **Chroń/Czułość**  >  **Pomoc i opinie**.
3. Kliknij **pozycję Eksportuj dzienniki**.
4. Zapisz dzienniki do wybranej lokalizacji i dołącz je do tego żądania usługi.

Dodatkowe zasoby:

- [Jak skonfigurować etykietę dla oznaczeń wizualnych dla usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Zapoznaj się z dokumentacją usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Używanie etykiet czułości w aplikacjach pakietu Office](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)


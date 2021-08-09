---
title: 'AIP: Zasady nie zachowują się zgodnie z oczekiwaniami'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934303"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Zasady nie zachowują się zgodnie z oczekiwaniami

Azure Information Protection: Zasady nie zachowują się zgodnie z oczekiwaniami, zobacz następujące zalecane wskazówki dotyczące różnych problemów z zasadami:

1. Jeśli masz problemy z oznaczeniami wizualnymi, zapoznaj się z [tematem Kiedy](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)są stosowane oznaczenia wizualne .
2. Jeśli masz problemy z automatycznym oznaczaniem etykiet, zapoznaj się z tematem Jak skonfigurować warunki dla klasyfikacji automatycznej i zalecanej dla usługi [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Czego szukać w przypadku typów informacji [poufnych.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Jeśli masz problemy z ochroną natywnych/plików P, sprawdź [konfigurację interfejsu API plików.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Sprawdź, czy używasz zasad o określonym zakresie, które nie są poprawnie skonfigurowane: [Jak skonfigurować zasady usługi Azure Information Protection dla określonych użytkowników przy użyciu zasad o określonym zakresie](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Jeśli automatyczne oznaczanie etykiet nie działa w programie Outlook podczas dołączania dokumentu oznaczonego etykietą, sprawdź, czy funkcja DRMEncryptProperty nie jest zdefiniowana w sposób opisany tutaj: Ustawienia rejestru [usługi IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)dla zabezpieczeń.

Jeśli nadal występują problemy, zbierz dzienniki klienta usługi Azure Information Protection i dołącz wyeksportowane dzienniki do tego biletu.

1. Otwórz dokument pakietu Office lub utwórz nową wiadomość e-mail w programie Outlook.
2. Kliknij przycisk **Ochrona/wrażliwość** > **Pomoc i opinie**.
3. Kliknij przycisk **Eksportuj dzienniki.**.
4. Zapisz dzienniki w wybranej lokalizacji i dołącz je do tego żądania usługi.

Dodatkowe zasoby:

- [Jak skonfigurować etykietę oznaczania wizualnego dla usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Przejrzyj dokumentację usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Używanie etykiet wrażliwości w Microsoft 365 aplikacjach](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)


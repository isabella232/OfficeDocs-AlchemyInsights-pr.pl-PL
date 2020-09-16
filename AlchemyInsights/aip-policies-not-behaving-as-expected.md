---
title: 'Podzasada: zasady niezachowuje się zgodnie z oczekiwaniami'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663199"
---
# <a name="aip-policies-not-behaving-as-expected"></a>Podzasada: zasady niezachowuje się zgodnie z oczekiwaniami

Ochrona informacji na platformie Azure: zasady nie zachowuje się zgodnie z oczekiwaniami, zapoznaj się z poniższymi wskazówkami dotyczącymi różnych zagadnień dotyczących zasad:

1. Jeśli występują problemy z oznaczeniami wizualnymi, sprawdź, czy [zostaną zastosowane oznaczenia wizualne](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Jeśli występują problemy z automatycznym oznaczaniem etykietami, zobacz [Konfigurowanie warunków automatycznej i zalecanej klasyfikacji usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) oraz tego [, co szukają typy informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Jeśli masz problemy z ochroną w trybie macierzystym/Pfileym, sprawdź [konfigurację interfejsu API pliku](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Sprawdzanie, czy są używane zasady dotyczące zakresu, które nie są poprawnie skonfigurowane: [jak skonfigurować zasady usługi Azure Information Protection dla określonych użytkowników przy użyciu zasad dotyczących zakresu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Jeśli automatyczne etykietowanie nie działa w programie Outlook podczas dołączania dokumentu opatrzonego etykietą, sprawdź, czy DRMEncryptProperty nie jest zdefiniowany w następujący sposób: [Ustawienia rejestru usługi IRM dotyczące zabezpieczeń](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Jeśli nadal występują problemy, Zbierz dzienniki klienta usługi Azure Information Protection i Dołącz wyeksportowane dzienniki do tego biletu.

1. Otwórz dokument pakietu Office lub Utwórz nową wiadomość e-mail w programie Outlook.
2. Kliknij pozycję Pomoc dotycząca **ochrony/wrażliwości**  >  **i opinie**.
3. Kliknij pozycję **Eksportuj dzienniki**.
4. Zapisz dzienniki w wybranym miejscu, a następnie dołącz je do tego żądania usługi.

Dodatkowe zasoby:

- [Jak skonfigurować etykietę wizualnych oznaczeń dla usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Przegląd dokumentacji dotyczącej ochrony informacji platformy Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Używanie etykiet liter w aplikacjach Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)


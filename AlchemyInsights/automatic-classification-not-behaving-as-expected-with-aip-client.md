---
title: Automatyczna klasyfikacja nie zachowuje się zgodnie z oczekiwaniami z klientem AIP
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
- "4373"
ms.openlocfilehash: 95a994d6a49ee8737a6ebcb196314f92776d8482
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493179"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatyczna klasyfikacja nie zachowuje się zgodnie z oczekiwaniami z klientem AIP

Automatyczna klasyfikacja nie zachowuje się zgodnie z oczekiwaniami, należy użyć następujących zalecanych wskazówek:

1. Jeśli masz problemy z automatycznym etykietowaniem, zobacz [Jak skonfigurować warunki automatycznej i zalecanej klasyfikacji dla usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i czego szukają [typy poufnych informacji.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
2. Sprawdź, czy używasz zasad o określonym zakresie, które nie są poprawnie skonfigurowane: [Jak skonfigurować zasady usługi Azure Information Protection dla określonych użytkowników przy użyciu zasad o określonym zakresie.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. Jeśli automatyczne etykietowanie nie działa w programie Outlook podczas dołączania dokumentu z etykietą, sprawdź, czy `DRMEncryptProperty` nie jest zdefiniowany zgodnie z opisem w tym miejscu: [Ustawienia rejestru usługi IRM dla zabezpieczeń](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Jeśli użyto [wbudowanych typów informacji](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) dla zasad usługi Azure Information Protection, sprawdź, czy zawartość jest zgodna z oczekiwanym formatem.
5. Sprawdź, czy etykieta jest odpowiednio skonfigurowana dla **automatycznego** lub **zalecanego**. (Automatyczne**etykietowanie** jest dostępne dla wszystkich aplikacji pakietu Office, podczas gdy **zalecane** jest dostępne dla wszystkich aplikacji pakietu Office z wyjątkiem programu Outlook).
6. Nie można używać automatycznej klasyfikacji dla dokumentów i wiadomości e-mail, które wcześniej były ręcznie oznaczone lub wcześniej automatycznie oznaczone wyższą klasyfikacją.  Aby uzyskać więcej informacji, zobacz: [Jak stosowane są etykiety automatyczne lub zalecane](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Jeśli nadal występują problemy, zbieraj dzienniki klientów usługi Azure Information Protection i dołączaj eksportowane dzienniki do biletu pomocy technicznej. Aby wyeksportować dzienniki usługi Azure Information Protection:
    - Otwórz dokument pakietu Office lub utwórz nową wiadomość e-mail w programie Outlook.
    - Kliknij pozycję **Chroń/Czułość**  >  **Pomoc i opinie**.
    - Kliknij **pozycję Eksportuj dzienniki**.
    - Zapisz dzienniki w wybranej lokalizacji i dołącz je do żądania usługi.

Aby uzyskać dodatkowe informacje, zobacz:

- [Jak skonfigurować warunki automatycznej i zalecanej klasyfikacji dla usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Instrukcje dotyczące typowych scenariuszy korzystających z usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Zapoznaj się z dokumentacją usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Przeglądanie subskrypcji i funkcji usługi Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Wymagania dotyczące usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Szybki start samouczek dotyczący usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Pobierz klienta usługi Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)

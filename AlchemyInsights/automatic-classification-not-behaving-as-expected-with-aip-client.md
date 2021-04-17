---
title: Automatyczna klasyfikacja nie działa zgodnie z oczekiwaniami w przypadku klientów usługi AIP
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
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820908"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatyczna klasyfikacja nie działa zgodnie z oczekiwaniami w przypadku klientów usługi AIP

Automatyczna klasyfikacja nie działa zgodnie z oczekiwaniami, skorzystaj z następujących zalecanych wskazówek:

1. Jeśli masz problemy z automatycznym etykietowaniem, zobacz [Jak skonfigurować warunki automatycznej i zalecanej klasyfikacji dla usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i [Jakie są poszukiwane typy informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Sprawdź, czy używasz zasad o określonym zakresie, które nie są poprawnie skonfigurowane: [Jak skonfigurować zasady usługi Azure Information Protection dla określonych użytkowników przy użyciu zasad o określonym zakresie](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Jeśli automatyczne etykietowanie nie działa w programie Outlook podczas dołączania dokumentu z etykietą, sprawdź, czy `DRMEncryptProperty`nie jest to zdefiniowane w sposób opisany tutaj:[Ustawienia rejestru usługi IRM dotyczące zabezpieczeń](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Jeśli użyto [wbudowanych typów informacji](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) dla zasad usługi Azure Information Protection, sprawdź, czy zawartość jest zgodna z oczekiwanym formatem.
5. Sprawdź, czy etykiety są odpowiednio skonfigurowane jako **Automatyczne** lub **Zalecane**. (**Automatyczne** etykietowanie jest dostępne dla wszystkich aplikacji platformy Microsoft 365, natomiast **Zalecane** jest dostępne dla wszystkich aplikacji platformy Microsoft 365 z wyjątkiem programu Outlook).
6. Nie można używać automatycznej klasyfikacji dokumentów i wiadomości e-mail, które wcześniej były ręcznie oznaczone lub poprzednio automatycznie oznaczane wyższą klasyfikacją.  Aby uzyskać więcej informacji, zobacz: [Jak są stosowane automatyczne lub zalecane etykiety](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Jeśli nadal występują problemy, zbierz dzienniki klienta usługi Azure Information Protection i dołącz wyeksportowane dzienniki do zgłoszenia do pomocy technicznej. Aby wyeksportować dzienniki usługi Azure Information Protection:
    - Otwórz dokument pakietu Office lub utwórz nową wiadomość e-mail w programie Outlook.
    - Kliknij przycisk **Ochrona/wrażliwość** > **Pomoc i opinie**.
    - Kliknij przycisk **Eksportuj dzienniki.**.
    - Zapisz dzienniki w wybranej lokalizacji i dołącz je do zgłoszenia serwisowego.

Aby uzyskać dodatkowe informacje, zobacz:

- [Jak skonfigurować warunki automatycznej i zalecanej klasyfikacji dla usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Poradniki dotyczące typowych scenariuszy korzystających z usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Przejrzyj dokumentację usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Przejrzyj subskrypcje usługi Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Wymagania dotyczące usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Samouczek Szybki start dotyczący usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Pobierz klienta usługi Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)

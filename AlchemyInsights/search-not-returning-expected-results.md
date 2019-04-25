---
title: 1491-Search-not-Returning-expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383845"
---
# <a name="content-search-not-returning-expected-results"></a>Przeszukiwanie zawartości nie zwraca wyników oczekiwanych

Podczas uruchamiania wyszukiwania zawartości z & zabezpieczeń usługi Office 365 Centrum zgodności, może pojawić się nieoczekiwanych wyników. Należy wziąć pod uwagę następujące rzeczy, które mogą wpływać na wyniki wyszukiwania:

- **Lokalizacje zawartości i warunki wyszukiwania**: Upewnij się, wybraniu odpowiedniej lokalizacji zawartości i warunki wyszukiwania. Jeśli uruchomiono dużych wyszukiwania (z wielu lokalizacji), należy rozważyć rozdzielenie go na wielu wyszukiwań.

- **Częściowo indeksowanych elementów**: [częściowo indeksowanych elementów](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) ze skrzynek pocztowych są uwzględniane w wynikach wyszukiwania szacowany. Jednak częściowo indeksowane elementy z witryn programu SharePoint i OneDrive nie są uwzględniane podczas szacowania wyszukiwania.

- **Wyszukiwanie błędów**: podczas wyszukiwania dużą liczbę skrzynek pocztowych (ponad 100 000 skrzynek pocztowych), mogą wystąpić błędy wyszukiwania, z kodami błędów, takich jak CS008-009 i CS012-002). W takim przypadku ponów próbę wyszukiwania tylko dla lokalizacji zawartości nie powiodło się. Zobacz [Ten artykuł](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) , aby uzyskać więcej informacji.

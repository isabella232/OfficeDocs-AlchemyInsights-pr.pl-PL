---
title: 1491-search-not-returning-expected-results 1491-search-not-returning-expected-results 1491-search-not-returning-expected-results 1
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709237"
---
# <a name="content-search-not-returning-expected-results"></a>Wyszukiwanie zawartości nie zwraca oczekiwanych wyników

Podczas uruchamiania wyszukiwania zawartości z Centrum zgodności & zabezpieczeń usługi Microsoft 365 mogą pojawić się nieoczekiwane wyniki wyszukiwania. Należy wziąć pod uwagę następujące kwestie, które mogą mieć wpływ na wyniki wyszukiwania:

- **Lokalizacje zawartości i warunki wyszukiwania:** upewnij się, że wybrano odpowiednie lokalizacje zawartości i warunki wyszukiwania. Jeśli uruchomiono duże wyszukiwanie (z wieloma lokalizacjami), rozważ podzielenie go na wiele wyszukiwań.

- **Elementy częściowo indeksowane**: [Elementy częściowo indeksowane](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) ze skrzynek pocztowych są uwzględniane w szacowanych wynikach wyszukiwania. Jednak elementy częściowo indeksowane z witryn w programie SharePoint i OneDrive nie są uwzględniane w szacowaniu wyszukiwania.

- **Błędy wyszukiwania:** Podczas przeszukiwania dużej liczby skrzynek pocztowych (ponad 100 000 skrzynek pocztowych) mogą pojawić się błędy wyszukiwania, z kodami błędów, takimi jak CS008-009 i CS012-002). W takim przypadku ponów próbę wyszukiwania tylko dla lokalizacji zawartości, które nie powiodło się. Zobacz [ten artykuł,](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) aby uzyskać więcej informacji.

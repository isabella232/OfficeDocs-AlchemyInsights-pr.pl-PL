---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052720"
---
# <a name="content-search-not-returning-expected-results"></a>Wyszukiwanie zawartości nie zwraca oczekiwanych wyników

Podczas uruchamiania przeszukiwań zawartości z centrum Microsoft 365 zabezpieczeń & zgodności mogą pojawić się nieoczekiwane wyniki wyszukiwania. Rozważ następujące kwestie, które mogą mieć wpływ na wyniki wyszukiwania:

- **Lokalizacje zawartości i warunki wyszukiwania:** upewnij się, że zostały wybrane odpowiednie lokalizacje zawartości i warunki wyszukiwania. Jeśli uruchomiono duże wyszukiwanie (z wieloma lokalizacjami), rozważ podzielenie go na wiele wyszukiwań.

- **Elementy częściowo indeksowane:**  [Elementy częściowo indeksowane](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) ze skrzynek pocztowych są uwzględniane w szacowanych wynikach wyszukiwania. Elementy częściowo indeksowane z witryn w witrynach SharePoint i OneDrive nie są uwzględniane w szacowanym wyszukiwaniu.

- **Błędy** wyszukiwania: Podczas wyszukiwania dużej liczby skrzynek pocztowych (ponad 100 000 skrzynek pocztowych) mogą wystąpić błędy wyszukiwania z kodami błędów, takimi jak CS008-009 i CS012-002). W takim przypadku ponów próbę wyszukiwania tylko lokalizacji zawartości, których dotyczy niepowodzenie. Aby  [uzyskać więcej informacji,](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) zobacz ten artykuł.

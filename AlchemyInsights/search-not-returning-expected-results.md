---
title: 1491 — wyniki wyszukiwania, nieoczekiwane
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740484"
---
# <a name="content-search-not-returning-expected-results"></a>Funkcja wyszukiwania zawartości nie zwraca oczekiwanych wyników

Podczas uruchamiania wyszukiwania zawartości z poziomu Centrum zgodności z & zabezpieczeniami programu Microsoft 365 mogą być wyświetlane nieoczekiwane wyniki wyszukiwania. Uwzględnij następujące kwestie, które mogą mieć wpływ na wyniki wyszukiwania:

- **Lokalizacje zawartości i warunki wyszukiwania**: Upewnij się, że wybrano odpowiednie lokalizacje zawartości i warunki wyszukiwania. Jeśli uruchomiono duże wyszukiwanie (z wieloma lokalizacjami), warto je podzielić na wiele wyszukiwań.

- **Częściowo indeksowane elementy**:  [częściowo indeksowane elementy](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) z skrzynek pocztowych są uwzględniane w szacowanych wynikach wyszukiwania. Jednak częściowo indeksowane elementy z witryn w programie SharePoint i w usłudze OneDrive nie są uwzględniane w szacowaniu wyszukiwania.

- **Błędy wyszukiwania**: podczas wyszukiwania dużej liczby skrzynek pocztowych (ponad 100 000 skrzynek pocztowych) możesz otrzymywać błędy wyszukiwania, korzystając z kodów błędów, takich jak CS008-009 i CS012-002). W takim przypadku ponów wyszukiwanie tylko w przypadku niepowodzenia lokalizacji zawartości. Aby uzyskać więcej informacji, zobacz  [ten artykuł](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

---
title: Określenie adresu IP i klienta w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539039"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Określenie adresu IP i klienta w dziennikach inspekcji

Adres IP, który odpowiada do działania przez użytkownika usługi Office 365 lub administratora systemu jest wyświetlane w dziennikach inspekcji. Rejestrowane są również informacje klienta. Poniżej przedstawiono kroki, aby takie informacje identyfikacyjne

1. Zaloguj się do [Centrum zgodności Office 365 zabezpieczeń &](https://protection.office.com/).

2. Przejdź do **wyszukiwania** > stronę**przeszukiwania dzienników inspekcji** .

   Jeśli interesują Cię określone działanie, wybierz go z listy **działań** . W przeciwnym razie zostaną zwrócone wszystkie działania dla wybranego użytkownika (ustawienie domyślne).

   **Uwaga**: niektóre rodzaje działalności mogą nie być dostępne w menu **działań** ; Jednakże inspekcja tych elementów zostaną zwrócone, jeśli **Pokaż wyniki dla wszystkich działalności** jest wybrany (ustawienie domyślne).

3. Określ nazwę użytkownika w polu **Użytkownicy** , wybierz zakres dat odpowiednie działania i kliknij przycisk **Wyszukaj**.

W wynikach można zobaczyć adres IP dla tego działania w okienku wyników. Wybierz rekord audytu, aby zobaczyć szczegółowe informacje w menu wysuwane **Szczegóły** (na przykład klienta, użytkownika, która wykonywana akcja, itp.).

Aby uzyskać więcej informacji zobacz [Znajdowanie adresu IP komputera umożliwia dostęp do skierowanego na to konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).

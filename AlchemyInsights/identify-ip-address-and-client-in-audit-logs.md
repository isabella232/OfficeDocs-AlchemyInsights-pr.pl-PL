---
title: Określenie adresu IP i klienta w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909443"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Określenie adresu IP i klienta w dziennikach inspekcji

Adres IP, który odpowiada do działania przez użytkownika lub administratora jest wyświetlane w dziennikach inspekcji. Rejestrowane są również informacje klienta. Poniżej przedstawiono kroki, aby takie informacje identyfikacyjne

1. Zaloguj się do [Centrum zgodności Office 365 zabezpieczeń &](https://protection.office.com/)

2. Kliknij przycisk **Wyszukaj i dochodzenia** i wybierz **Przeszukiwania dzienników inspekcji**.

   Jeśli interesują Cię określone działanie, wybierz go z listy **działań** . W przeciwnym razie zostaną zwrócone wszystkie działania dla wybranego użytkownika (ustawienie domyślne).

   **Uwaga**: niektóre rodzaje działalności mogą nie być dostępne w menu **działań** ; Jednakże inspekcja tych elementów zostaną zwrócone, jeśli **Pokaż wyniki dla wszystkich działalności** jest wybrany (ustawienie domyślne).

3. Określ nazwę użytkownika w polu **Użytkownicy** , wybierz zakres dat odpowiednie działania i kliknij przycisk **Wyszukaj**.

W wynikach można zobaczyć adres IP dla tego działania w okienku wyników. Wybierz rekord audytu, aby zobaczyć szczegółowe informacje w menu wysuwane **Szczegóły** (na przykład klienta, użytkownika, która wykonywana akcja, itp.).

Aby uzyskać więcej informacji zobacz [Znajdowanie adresu IP komputera umożliwia dostęp do skierowanego na to konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).

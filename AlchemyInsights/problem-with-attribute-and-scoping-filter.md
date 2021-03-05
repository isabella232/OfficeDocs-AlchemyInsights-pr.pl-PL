---
title: Problem z atrybutem i filtrem zakresu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481897"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problem z atrybutami i filtrowaniem zakresu

**Problem z wartościami upn powodujące konflikt**

W dzień roboczy inicjowania obsługi administracyjnej użytkownika usługi AD w trybie inicjowania obsługi administracyjnej użytkownika usługi AD jest wyświetlany komunikat o błędzie **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.** Operacja nie powiodła się, ponieważ główna wartość w zakresie dodatku/modyfikacji nie jest unikatowa dla całego lasu. Szczegóły błędu: **CONSTRAINT_ATT_TYPE — userPrincipalName.**

Wartość **userPrincipalName,** która próbuje ustawić łącznik dzień roboczy podczas tworzenia konta użytkownika usługi AD, już istnieje w docelowej domenie usługi AD. Oznacza to, że użytkownik (1) już istnieje i nie udało się sprawdzić pasującego identyfikatora przez użytkownika lub (2) reguła generowania upn wygenerowała wartość kolidującą.

Poniżej podano sugerowane kroki rozwiązania problemu:

Jeśli użytkownik już istnieje, a nie udało się połączyć konta w dzień roboczy z kontem usługi Active Directory, sprawdź, czy zgodny atrybut identyfikatora (zwykle **identyfikator** pracownika) zarówno w dzień roboczy, jak i w usłudze AD ma dokładne dopasowanie. Jeśli nie ma dopasowania, problem z danymi należy rozwiązać. Jeśli na przykład identyfikator pracownika w dniu pracy to 001052, a w u użytkownikach AD jest to 1052, aparat obsługi administracyjnej nie połączy tych dwóch kont i spróbuje utworzyć użytkownika, który już istnieje. W tym przypadku rozwiązaniem jest zmiana wartości **Identyfikator** pracownika w u użytkownikach w u użytkownikach AD tak, aby zawierała zera wiodące, aby była równa 001052.
Jeśli wyrażenie generujące upn nie generuje unikatowej wartości, rozważ każdorazowe wygenerowanie unikatowej wartości przy użyciu funkcji de duplikowania **SelectUniqueValue.**

**Inicjowanie obsługi użytkowników w dni robocze do usługi AD nie powoduje ustawienia wartości atrybutu menedżera dla konta użytkownika usługi AD**

Zadanie inicjowania obsługi użytkowników usługi AD w dzień roboczy nie ustawia wartości atrybutu **menedżera** dla kont użytkowników usługi AD. Takie zachowanie jest widoczne w dwóch scenariuszach:

1. Kierownika w dzień roboczy nie można rozpoznać do odpowiadającego mu konta użytkownika usługi AD, ponieważ menedżer nie znajduje się w zakresie.
2. W **scenariuszu z wieloma domenami** usługi AD kierownik w dzień roboczy nie występuje w tej samej domenie co użytkownik.

Aby rozwiązać ten problem, spróbuj wykonać następujące czynności:

1. Jeśli zdefiniowano zakres filtrów, najpierw sprawdź, czy menedżer znajduje się w zakresie i spełnia warunki określone w klauzuli zakresu. Jeśli menedżer nie spełnia filtru zakresu, zmień filtr tak, aby menedżer również był w zakresie operacji inicjowania obsługi administracyjnej.
2. Jeśli masz wiele domen usługi AD, łącznik ma znane ograniczenie, które ma problemy z rozwiązywanie odwołań między menedżerami domen.

Aby uzyskać więcej szczegółowych informacji na temat konfigurowania dnia roboczego dla automatycznego inicjowania obsługi, zobacz Samouczek: Konfigurowanie dnia roboczego dla [automatycznego inicjowania obsługi administracyjnej użytkowników.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)














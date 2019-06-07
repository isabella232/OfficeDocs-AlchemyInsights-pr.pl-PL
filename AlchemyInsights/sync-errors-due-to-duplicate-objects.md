---
title: 902 (błędy synchronizacji z powodu zduplikowane obiekty)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758005"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Błędy synchronizacji ze względu na powielanie obiektów

Może pojawić się jeden z następujących komunikatów o błędach po zakończeniu synchronizacji katalogów:

- Nie można zaktualizować tego obiektu w witrynie Microsoft Online Services, ponieważ następujące atrybuty skojarzone z tym obiektem wartości, które mogą być już skojarzony z innym obiektem w katalogu lokalnym.

- Synchronizowanego obiektu z tym samym adresem proxy już istnieje w katalogu programu Microsoft Online Services.

- Nie można zaktualizować tego obiektu, ponieważ następujące atrybuty skojarzone z tym obiektem wartości, które mogą być już skojarzony z innym obiektem w sieci usługi katalogu lokalnego: UserPrincipalName.

Aby zidentyfikować i rozwiązać ten problem, Pobierz i uruchom [Narzędzie korygowania błędów IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Aby uzyskać więcej informacji zobacz [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).

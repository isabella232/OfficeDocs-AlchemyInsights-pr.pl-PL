---
title: 902 (Błędy synchronizacji spowodowane zduplikowanymi obiektami)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767144"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Błędy synchronizacji spowodowane duplikatami obiektów

Po zakończeniu synchronizacji katalogów w usłudze Microsoft 365 może zostać wyświetlony jeden z następujących komunikatów o błędach:

- Nie można zaktualizować tego obiektu w usługach Microsoft Online Services, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w katalogu lokalnym.

- Zsynchronizowany obiekt o tym samym adresie serwera proxy już istnieje w katalogu usług Online Services firmy Microsoft.

- Nie można zaktualizować tego obiektu, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w lokalnych usługach katalogowych: UserPrincipalName.

Aby zidentyfikować i rozwiązać problem, pobierz i uruchom [narzędzie do korygowania błędów IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Aby uzyskać więcej informacji, zobacz [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).

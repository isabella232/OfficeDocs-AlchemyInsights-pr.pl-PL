---
title: 902 (Błędy synchronizacji spowodowane zduplikowanymi obiektami)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998804"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Błędy synchronizacji spowodowane zduplikowanymi obiektami

Po zakończeniu synchronizacji katalogów w programie Microsoft 365:

- Nie można zaktualizować tego obiektu w usługach Microsoft Online Services, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w katalogu lokalnym.

- Obiekt zsynchronizowany z tym samym adresem serwera proxy już istnieje w katalogu usług Microsoft Online Services.

- Nie można zaktualizować tego obiektu, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w lokalnych usługach katalogowych: UserPrincipalName.

Aby zidentyfikować i rozwiązać ten problem, pobierz i uruchom narzędzie naprawy błędów synchronizacji katalogów narzędzia [IdFix.](https://github.com/Microsoft/idfix)

Aby uzyskać więcej informacji, [zobacz KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)

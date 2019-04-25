---
title: 902 (błędy synchronizacji z powodu zduplikowane obiekty)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420909"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Błędy synchronizacji ze względu na powielanie obiektów

Może pojawić się jeden z następujących komunikatów o błędach po zakończeniu synchronizacji katalogów:

- Nie można zaktualizować tego obiektu w witrynie Microsoft Online Services, ponieważ następujące atrybuty skojarzone z tym obiektem wartości, które mogą być już skojarzony z innym obiektem w katalogu lokalnym.

- Synchronizowanego obiektu z tym samym adresem proxy już istnieje w katalogu programu Microsoft Online Services.

- Nie można zaktualizować tego obiektu, ponieważ następujące atrybuty skojarzone z tym obiektem wartości, które mogą być już skojarzony z innym obiektem w sieci usługi katalogu lokalnego: UserPrincipalName.

Aby zidentyfikować i rozwiązać ten problem, Pobierz i uruchom [Narzędzie korygowania błędów IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Aby uzyskać więcej informacji zobacz [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).

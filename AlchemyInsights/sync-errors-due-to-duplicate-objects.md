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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708072"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Błędy synchronizacji spowodowane zduplikowanymi obiektami

Po zakończeniu synchronizacji katalogów na usłudze Microsoft 365 może zostać wyświetlony jeden z następujących komunikatów o błędzie:

- Nie można zaktualizować tego obiektu w usługach Microsoft Online Services, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w katalogu lokalnym.

- Obiekt zsynchronizowany z tym samym adresem serwera proxy już istnieje w katalogu usług Microsoft Online Services.

- Nie można zaktualizować tego obiektu, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w lokalnych usługach katalogowych: UserPrincipalName.

Aby zidentyfikować i rozwiązać ten problem, pobierz i uruchom narzędzie do rozwiązywania problemów [narzędzia DirSync narzędzia IdFix.](https://github.com/Microsoft/idfix)

Aby uzyskać więcej informacji, zobacz [ARTYKUŁ KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)

---
title: Dynamics 365 formularze reguły biznesowe-reguły biznesowe nie wypalania dla formularza
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769349"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Zdarzenie OnChange nie występuje, jeśli pole jest zmieniane programowo

Zdarzenie *OnChange* nie występuje, jeśli pole jest zmieniane programowo przy użyciu *atrybutu.* [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metody. Jeśli chcesz obsługi zdarzeń *OnChange* zdarzenie, aby uruchomić po ustawieniu wartości należy użyć *formcontext. Data. Entity atrybutu* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metody w kodzie.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)

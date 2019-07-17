---
title: Reguły biznesowe — reguła biznesowa nie uruchomiono formularza tworzy Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748343"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Zdarzenie OnChange nie występuje, jeśli pole zostanie zmieniona programowo

Zdarzenie *OnChange* nie występuje, jeśli pole zostanie zmieniona programowo przy użyciu *atrybutu.* Metoda [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Jeśli chcesz, aby programy obsługi zdarzeń dla zdarzenia *PrzyZmianie* uruchomiony po ustawieniu wartości, należy użyć *atrybutu formContext.data.entity.* Metoda [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) w kodzie.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)

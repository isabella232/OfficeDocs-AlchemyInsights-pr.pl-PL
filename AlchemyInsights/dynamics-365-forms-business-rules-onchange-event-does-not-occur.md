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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529029"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Zdarzenie OnChange nie występuje, jeśli pole zostanie zmieniona programowo

Zdarzenie *OnChange* nie występuje, jeśli pole zostanie zmieniona programowo przy użyciu *atrybutu.* Metoda [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Jeśli chcesz, aby programy obsługi zdarzeń dla zdarzenia *PrzyZmianie* uruchomiony po ustawieniu wartości, należy użyć *atrybutu formContext.data.entity.* Metoda [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) w kodzie.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)

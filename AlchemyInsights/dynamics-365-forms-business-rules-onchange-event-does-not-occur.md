---
title: Reguły biznesowe formularzy usługi Dynamics 365 — nie można odtworzyć reguły biznesowej dla formularza
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947309"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Zdarzenie OnChange nie występuje, jeśli pole jest zmieniane programowo

Zdarzenie *OnChange* (PrzyZmianie) nie występuje, jeśli pole zostało zmienione programowo przy użyciu *tego atrybutu.* [metoda setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Aby programy obsługi zdarzeń zdarzenia *OnChange* uruchamiały się po skonfigurowaniu wartości, należy w kodzie użyć metody *atrybutu formContext.data.entity* [fireOnchange.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)

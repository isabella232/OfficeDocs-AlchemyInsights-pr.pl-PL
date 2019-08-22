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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="a0af9-102">Zdarzenie OnChange nie występuje, jeśli pole zostanie zmieniona programowo</span><span class="sxs-lookup"><span data-stu-id="a0af9-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="a0af9-103">Zdarzenie *OnChange* nie występuje, jeśli pole zostanie zmieniona programowo przy użyciu *atrybutu.* Metoda [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="a0af9-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="a0af9-104">Jeśli chcesz, aby programy obsługi zdarzeń dla zdarzenia *PrzyZmianie* uruchomiony po ustawieniu wartości, należy użyć *atrybutu formContext.data.entity.* Metoda [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) w kodzie.</span><span class="sxs-lookup"><span data-stu-id="a0af9-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)

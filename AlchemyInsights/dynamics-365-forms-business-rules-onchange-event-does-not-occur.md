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
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769349"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="80348-102">Zdarzenie OnChange nie występuje, jeśli pole jest zmieniane programowo</span><span class="sxs-lookup"><span data-stu-id="80348-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="80348-103">Zdarzenie *OnChange* nie występuje, jeśli pole jest zmieniane programowo przy użyciu *atrybutu.* [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metody.</span><span class="sxs-lookup"><span data-stu-id="80348-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="80348-104">Jeśli chcesz obsługi zdarzeń *OnChange* zdarzenie, aby uruchomić po ustawieniu wartości należy użyć *formcontext. Data. Entity atrybutu* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metody w kodzie.</span><span class="sxs-lookup"><span data-stu-id="80348-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)

---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813770"
---
# <a name="error-attributevaluemustbeunique"></a>Błąd: AttributeValueMustBeUnique

Najczęstszą przyczyną błędu AttributeValueMustBeUnique są dwa obiekty o różnych atrybutach SourceAnchor (immutableId) o tej samej wartości atrybutów ProxyAddresses i/lub UserPrincipalName. Aby naprawić błąd AttributeValueMustBeUnique:
  
1. Zidentyfikuj zduplikowane wartości proxyAddresses, userPrincipalName lub inną wartość atrybutu, która powoduje błąd. Określ także, które (lub więcej) obiektów biorą udział w konflikcie. Raport wygenerowany przez narzędzie Azure AD Connect Health do synchronizacji może pomóc w zidentyfikowaniu tych dwóch obiektów.
    
2. Określ obiekt, który powinien mieć zduplikowaną wartość, a który nie.
    
3. Usuń zduplikowaną wartość z obiektu, który NIE powinien mieć tej wartości. Zwróć uwagę, że należy wprowadzić zmiany w katalogu, z którego pochodzi obiekt. W niektórych przypadkach może być konieczne usunięcie jednego z obiektów, w przypadku których występuje konflikt.
    
4. Jeśli dokonano zmiany w lokalnej usłudze AD, zechć, aby program Azure AD Connect zsynchronizował zmianę błędu, aby rozwiązać ten problem.
    


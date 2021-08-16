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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002130"
---
# <a name="error-attributevaluemustbeunique"></a>Błąd: AttributeValueMustBeUnique

Najczęstszą przyczyną błędu AttributeValueMustBeUnique są dwa obiekty o różnych atrybutach SourceAnchor (immutableId) o tej samej wartości atrybutów ProxyAddresses i/lub UserPrincipalName. Aby naprawić błąd AttributeValueMustBeUnique:
  
1. Zidentyfikuj zduplikowane wartości proxyAddresses, userPrincipalName lub inną wartość atrybutu, która powoduje błąd. Określ także, które (lub więcej) obiektów biorą udział w konflikcie. Raport wygenerowany przez usługę Azure AD Połączenie kondycji synchronizacji może pomóc w zidentyfikowaniu tych dwóch obiektów.
    
2. Określ obiekt, który powinien mieć zduplikowaną wartość, a który nie.
    
3. Usuń zduplikowaną wartość z obiektu, który NIE powinien mieć tej wartości. Zwróć uwagę, że należy wprowadzić zmiany w katalogu, z którego pochodzi obiekt. W niektórych przypadkach może być konieczne usunięcie jednego z obiektów, w przypadku których występuje konflikt.
    
4. Jeśli dokonano zmiany w lokalnej usłudze AD, zechć, aby usługa Azure AD Połączenie zsynchronizować zmianę, aby błąd został rozwiązany.
    


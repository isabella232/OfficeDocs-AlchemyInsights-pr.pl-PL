---
title: Błąd AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709161"
---
# <a name="error-attributevaluemustbeunique"></a>Błąd: AttributeValueMustBeUnique

Najczęstszą przyczyną błędu AttributeValueMustBeUnique jest dwa obiekty z różnymi SourceAnchor (immutableId) mają taką samą wartość dla atrybutów ProxyAddresses i/lub UserPrincipalName. Aby rozwiązać błąd AttributeValueMustBeUnique:
  
1. Zidentyfikuj zduplikowaną wartość proxyAddresses, userPrincipalName lub innej wartości atrybutu powodującej błąd. Określ również, które dwa (lub więcej) obiekty są związane z konfliktem. Raport wygenerowany przez usługę Azure AD Connect Health na potrzeby synchronizacji może pomóc w zidentyfikowaniu tych dwóch obiektów.
    
2. Określ, który obiekt ma nadal zawierać zduplikowaną wartość, a który obiekt nie powinien.
    
3. Usuń zduplikowaną wartość z obiektu, który nie powinien mieć tej wartości. Należy pamiętać, że należy wprowadzić zmianę w katalogu, z którego pochodzi obiekt źródłowy. W niektórych przypadkach może być konieczne usunięcie jednego z obiektów powodujących konflikt.
    
4. Jeśli zmiana została wprowadzona w lokalnej usłudze AD, zezwól usłudze Azure AD Connect na synchronizowanie zmiany błędu w celu naprawienia błędów.
    


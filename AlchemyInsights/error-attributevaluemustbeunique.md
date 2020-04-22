---
title: Błąd AtrybutValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703184"
---
# <a name="error-attributevaluemustbeunique"></a>Błąd: AttributeValueMustBeUnique

Najczęstszą przyczyną attributeValueMustBeUnique błąd jest dwa obiekty z różnych SourceAnchor (immutableId) mają taką samą wartość dla ProxyAddresses i/lub UserPrincipalName atrybutów. Aby naprawić błąd AttributeValueMustBeUnique:
  
1. Zidentyfikuj zduplikowane proxyAddresses, userPrincipalName lub inną wartość atrybutu, która powoduje błąd. Należy również określić, które dwa (lub więcej) obiekty są zaangażowane w konflikt. Raport wygenerowany przez usługę Azure AD Connect Health do synchronizacji może pomóc w zidentyfikowaniu dwóch obiektów.
    
2. Określ, który obiekt powinien nadal mieć zduplikowaną wartość, a który nie powinien.
    
3. Usuń zduplikowaną wartość z obiektu, który NIE powinien mieć tej wartości. Należy zauważyć, że należy wprowadzić zmiany w katalogu, z którego pochodzi obiekt. W niektórych przypadkach może być konieczne usunięcie jednego z obiektów w konflikcie.
    
4. Jeśli w lokalnej usłudze AD została wyeksja lokalna, usługa Azure AD Connect zsynchronizowana ze zmianą błędu została naprawiona.
    


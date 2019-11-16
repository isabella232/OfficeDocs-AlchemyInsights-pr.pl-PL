---
title: Błąd AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36527033"
---
# <a name="error-attributevaluemustbeunique"></a>Błąd: AttributeValueMustBeUnique

Najczęstszym powodem dla AttributeValueMustBeUnique błąd jest dwa obiekty z różnych SourceAnchor (immutableId) mają taką samą wartość dla ProxyAddresses i/lub UserPrincipalName atrybuty. Aby naprawić błąd AttributeValueMustBeUnique:
  
1. Zidentyfikuj zduplikowane proxyAddresses, userPrincipalName lub inną wartość atrybutu, który jest przyczyną błędu. Również określić, które dwa (lub więcej) obiekty są zaangażowane w konflikt. Raport wygenerowany przez usługę Azure AD Connect Health do synchronizacji może pomóc w zidentyfikowaniu dwóch obiektów.
    
2. Określ, który obiekt powinien nadal mieć zduplikowane wartości i który obiekt nie powinien.
    
3. Usuń zduplikowana wartość z obiektu, który nie powinien mieć tej wartości. Należy pamiętać, że należy wprowadzić zmiany w katalogu, z którego pochodzi obiekt. W niektórych przypadkach może być konieczne usunięcie jednego z obiektów w konflikcie.
    
4. Jeśli wprowadzono zmiany w lokalnej usługi AD, pozwól Azure AD Connect zsynchronizować zmiany błędu, aby uzyskać stałe.
    


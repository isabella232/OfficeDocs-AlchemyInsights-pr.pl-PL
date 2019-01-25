---
title: Błąd AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499644"
---
# <a name="error-attributevaluemustbeunique"></a>Błąd: AttributeValueMustBeUnique

Najczęstszym powodem błędu AttributeValueMustBeUnique jest dwa obiekty o różnych SourceAnchor (immutableId) mają tę samą wartość dla atrybutów ProxyAddresses i/lub UserPrincipalName. Aby naprawić błąd AttributeValueMustBeUnique:
  
1. Zidentyfikować zduplikowane proxyAddresses, userPrincipalName lub inne wartości atrybutu, który jest przyczyną błędu. Również zidentyfikować obiekty, które dwóch (lub więcej) są zaangażowane w konflikcie. Raportu generowanych przez usługę Azure AD Connect Health dla synchronizacji może pomóc w zidentyfikowaniu dwóch obiektów.
    
2. Identyfikacji obiektu, który powinien w dalszym ciągu mają zduplikowane wartości i obiektu, który nie powinien.
    
3. Usuń zduplikowane wartości z obiektu, który nie powinien mieć tę wartość. Należy zauważyć, że należy wprowadzić zmianę w katalogu, gdzie pochodzą z obiektu. W niektórych przypadkach może być konieczne usunąć jeden z obiektów w konflikcie.
    
4. Jeśli wprowadzono zmiany w pomieszczeniach na AD Niech Azure Połącz AD synchronizacji zmian dla błędu uzyskać stałą.
    


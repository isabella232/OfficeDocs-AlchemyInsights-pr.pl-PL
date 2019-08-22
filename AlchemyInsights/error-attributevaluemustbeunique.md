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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527033"
---
# <a name="error-attributevaluemustbeunique"></a>Błąd: AttributeValueMustBeUnique

Najczęstszym powodem błędu AttributeValueMustBeUnique jest dwa obiekty o różnych SourceAnchor (immutableId) mają tę samą wartość dla atrybutów ProxyAddresses i/lub UserPrincipalName. Aby naprawić błąd AttributeValueMustBeUnique:
  
1. Zidentyfikować zduplikowane proxyAddresses, userPrincipalName lub inne wartości atrybutu, który jest przyczyną błędu. Również zidentyfikować obiekty, które dwóch (lub więcej) są zaangażowane w konflikcie. Raportu generowanych przez usługę Azure AD Connect Health dla synchronizacji może pomóc w zidentyfikowaniu dwóch obiektów.
    
2. Identyfikacji obiektu, który powinien w dalszym ciągu mają zduplikowane wartości i obiektu, który nie powinien.
    
3. Usuń zduplikowane wartości z obiektu, który nie powinien mieć tę wartość. Należy zauważyć, że należy wprowadzić zmianę w katalogu, gdzie pochodzą z obiektu. W niektórych przypadkach może być konieczne usunąć jeden z obiektów w konflikcie.
    
4. Jeśli wprowadzono zmiany w pomieszczeniach na AD Niech Azure Połącz AD synchronizacji zmian dla błędu uzyskać stałą.
    


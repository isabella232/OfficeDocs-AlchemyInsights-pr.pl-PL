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
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402713"
---
# <a name="error-attributevaluemustbeunique"></a>Błąd: AttributeValueMustBeUnique

Najczęstszym powodem błędu AttributeValueMustBeUnique jest dwa obiekty o różnych SourceAnchor (immutableId) mają tę samą wartość dla atrybutów ProxyAddresses i/lub UserPrincipalName. Aby naprawić błąd AttributeValueMustBeUnique:
  
1. Zidentyfikować zduplikowane proxyAddresses, userPrincipalName lub inne wartości atrybutu, który jest przyczyną błędu. Również zidentyfikować obiekty, które dwóch (lub więcej) są zaangażowane w konflikcie. Raportu generowanych przez usługę Azure AD Connect Health dla synchronizacji może pomóc w zidentyfikowaniu dwóch obiektów.
    
2. Identyfikacji obiektu, który powinien w dalszym ciągu mają zduplikowane wartości i obiektu, który nie powinien.
    
3. Usuń zduplikowane wartości z obiektu, który nie powinien mieć tę wartość. Należy zauważyć, że należy wprowadzić zmianę w katalogu, gdzie pochodzą z obiektu. W niektórych przypadkach może być konieczne usunąć jeden z obiektów w konflikcie.
    
4. Jeśli wprowadzono zmiany w pomieszczeniach na AD Niech Azure Połącz AD synchronizacji zmian dla błędu uzyskać stałą.
    


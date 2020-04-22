---
title: ConsistencyGuid / sourceAchor zachowanie
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705743"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAchor zachowanie

Usługa Azure AD Connect (wersja 1.1.524.0 i później) ułatwia teraz korzystanie z msDS-ConsistencyGuid jako sourceAnchor atrybut. Korzystając z tej funkcji, usługa Azure AD Connect automatycznie konfiguruje reguły synchronizacji na:
  
- Użyj msDS-ConsistencyGuid jako sourceAnchor atrybut dla user obiektów. ObjectGUID jest używany dla innych typów obiektów.
    
- Dla każdego danego lokalnego obiektu użytkownika usługi AD, którego atrybut msDS-ConsistencyGuid nie jest wypełniony, usługa Azure AD Connect zapisuje swoją wartość objectGUID z powrotem do atrybutu msDS-ConsistencyGuid w lokalnej usłudze Active Directory. Po wypełnieniu atrybutu msDS-ConsistencyGuid usługa Azure AD Connect eksportuje obiekt do usługi Azure AD.
    
 **Uwaga:** Po zaimportowaniu lokalnego obiektu usługi AD do usługi Azure AD Connect (czyli zaimportowane do obszaru łącznika usługi AD i rzutowane do metaverse), nie można już zmienić jego sourceAnchor wartość. Aby określić wartość sourceAnchor dla danego lokalnego obiektu USŁUGI AD, skonfiguruj jego atrybut msDS-ConsistencyGuid przed zaimportowaniem do usługi Azure AD Connect. 
  
Aby uzyskać więcej informacji na temat SourceAnchor i ConsistencyGuid, zobacz następujące: [Azure AD Connect: Pojęcia projektowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  


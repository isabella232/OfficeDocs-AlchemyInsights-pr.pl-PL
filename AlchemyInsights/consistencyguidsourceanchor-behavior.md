---
title: ConsistencyGuid/sourceAnchor behavior
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817002"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor behavior

Program Azure AD Connect (wersja 1.1.524.0 i po) teraz ułatwia użycie atrybutu msDS-ConsistencyGuid jako atrybutu sourceAnchor. Podczas korzystania z tej funkcji program Azure AD Connect automatycznie konfiguruje reguły synchronizacji do:
  
- Użyj atrybutu msDS-ConsistencyGuid jako atrybutu sourceAnchor dla obiektów User. Identyfikator OBJECTGUID jest używany w przypadku innych typów obiektów.
    
- W przypadku dowolnego lokalnego obiektu użytkownika usługi AD, którego atrybut msDS-ConsistencyGuid nie jest wypełniony, program Azure AD Connect zapisuje wartość objectGUID z powrotem w atrybutu msDS-ConsistencyGuid w lokalnej usłudze Active Directory. Po wypełnieniu atrybutu msDS-ConsistencyGuid program Azure AD Connect eksportuje obiekt do usługi Azure AD.
    
 **Uwaga:** Po zaimportowaniu lokalnego obiektu usługi AD do programu Azure AD Connect (czyli zaimportowania do obszaru łącznika usługi AD i wyeksportowanego do obiektu Metaverse) nie można już zmienić jego wartości sourceAnchor. Aby określić wartość sourceAnchor dla danego lokalnego obiektu usługi AD, skonfiguruj jej atrybut msDS-ConsistencyGuid przed zaimportowaniu do programu Azure AD Connect. 
  
Aby uzyskać więcej informacji na temat sourceAnchor i ConsistencyGuid, zobacz następujące informacje: [Azure AD Connect: koncepcje projektowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  


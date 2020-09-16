---
title: Zachowanie ConsistencyGuid/sourceAnchor
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756293"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Zachowanie ConsistencyGuid/sourceAnchor

Usługa Azure AD Connect (wersja 1.1.524.0 i późniejsza) ułatwia korzystanie z msDS-ConsistencyGuid jako atrybutu sourceAnchor. W przypadku korzystania z tej funkcji usługa Azure AD Connect automatycznie konfiguruje reguły synchronizacji:
  
- Użyj msDS-ConsistencyGuid jako atrybutu sourceAnchor dla obiektów użytkowników. ObjectGUID jest używana w przypadku innych typów obiektów.
    
- W przypadku dowolnego lokalnego obiektu użytkownika usługi AD, którego atrybut msDS-ConsistencyGuid nie jest wypełniony, usługa Azure AD Connect zapisuje swoją wartość objectGUID z powrotem w atrybucie msDS-ConsistencyGuid w lokalnej usłudze Active Directory. Po wypełnieniu atrybutu msDS-ConsistencyGuid, usługa Azure AD Connect następnie eksportuje obiekt do usługi Azure AD.
    
 **Uwaga:** Po zaimportowaniu lokalnego obiektu usługi AD do usługi Azure AD Connect (czyli zaimportowaniu go do przestrzeni łącznika usług AD w celu wydzielenia go na element Metaverse) nie można już zmienić jego wartości sourceAnchor. Aby określić wartość sourceAnchor dla określonego lokalnego obiektu usługi AD, skonfiguruj swój atrybut msDS-ConsistencyGuid przed zaimportowaniem go do usługi Azure AD Connect. 
  
Aby uzyskać więcej informacji na temat SourceAnchor i ConsistencyGuid, zapoznaj się z następującymi elementami: [Azure AD Connect: koncepcje dotyczące projektowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  


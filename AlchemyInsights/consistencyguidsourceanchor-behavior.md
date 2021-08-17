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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044350"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor behavior

Usługa Azure AD Połączenie (wersja 1.1.524.0 i nowsza) teraz ułatwia użycie atrybutu msDS-ConsistencyGuid jako atrybutu sourceAnchor. Podczas korzystania z tej funkcji usługa Azure AD Połączenie automatycznie konfiguruje reguły synchronizacji w celu:
  
- Użyj atrybutu msDS-ConsistencyGuid jako atrybutu sourceAnchor dla obiektów User. Identyfikator OBJECTGUID jest używany w przypadku innych typów obiektów.
    
- W przypadku dowolnego lokalnego obiektu użytkownika usługi AD, którego atrybut msDS-ConsistencyGuid nie jest wypełniony, usługa Azure AD Połączenie zapisuje jego wartość objectGUID z powrotem w atrybutu msDS-ConsistencyGuid w lokalnej usłudze Active Directory. Po wypełnieniu atrybutu msDS-ConsistencyGuid usługa Azure AD Połączenie następnie wyeksportowała obiekt do usługi Azure AD.
    
 **Uwaga:** Po zaimportowaniu lokalnego obiektu usługi AD do usługi Azure AD Połączenie (czyli zaimportowaniu do obszaru łącznika usługi AD i prognozowane do obiektu Metaverse) nie można już zmienić jego wartości sourceAnchor. Aby określić wartość sourceAnchor dla danego lokalnego obiektu usługi AD, skonfiguruj jej atrybut msDS-ConsistencyGuid przed zaimportowaniu do usługi Azure AD Połączenie. 
  
Aby uzyskać więcej informacji na temat sourceAnchor i ConsistencyGuid, zobacz następujące informacje: Usługa [Azure AD Połączenie: Koncepcje projektowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  


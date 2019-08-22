---
title: ConsistencyGuid / sourceAnchor zachowanie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517002"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor zachowanie

Azure AD Connect (wersja 1.1.524.0 i po) teraz ułatwia korzystanie z msDS-ConsistencyGuid jako atrybut sourceAnchor. Podczas korzystania z tej funkcji Azure AD Połącz automatycznie konfiguruje reguły synchronizacji:
  
- Użyj msDS-ConsistencyGuid jako atrybut sourceAnchor dla obiektów użytkowników. ObjectGUID jest używany dla innych typów obiektów.
    
- Dla danego lokalnego użytkownika AD obiektu, którego atrybut msDS-ConsistencyGuid nie jest wypełniona, Azure pisze Połącz AD jego wartość objectGUID z powrotem do atrybutu msDS-ConsistencyGuid w usłudze Active Directory w lokalnym. Po jest wypełniane atrybut msDS-ConsistencyGuid, Azure Połącz AD następnie eksportuje obiekt Azure AD.
    
 **Uwaga:** Raz lokalnego obiektu AD jest importowany do Azure Połącz AD (czyli przywożone do przestrzeni łączników AD i przewidywane do obiektu Metaverse), nie można już zmienić jego wartość sourceAnchor. Aby określić wartość sourceAnchor dla biorąc pod uwagę lokalnej AD obiektów, zanim to zostanie zaimportowane do Azure Połącz AD skonfigurować jego atrybut msDS-ConsistencyGuid. 
  
Aby uzyskać więcej informacji dotyczących SourceAnchor i ConsistencyGuid, odnoszą się do następujących: [Azure AD Connect: koncepcje projektowe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  


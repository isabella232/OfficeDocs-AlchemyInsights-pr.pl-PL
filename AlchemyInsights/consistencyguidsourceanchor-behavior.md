---
title: Zachowanie Konsystencyguid/sourceAnchor
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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36517002"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Zachowanie Konsystencyguid/sourceAnchor

Azure AD Connect (wersja 1.1.524.0 i After) teraz ułatwia korzystanie z msDS-Konsystencyguid jako atrybut sourceAnchor. Korzystając z tej funkcji, program Azure AD Connect automatycznie konfiguruje reguły synchronizacji do:
  
- Użyj msDS-Konsystencyguid jako atrybut sourceAnchor dla obiektów użytkownika. ObjectGUID jest używany dla innych typów obiektów.
    
- Dla dowolnego danego obiektu użytkownika AD lokalnego, którego atrybut msDS-Konsystencyguid nie jest wypełniona, program Azure AD Connect zapisuje jego wartość objectGUID z powrotem do atrybutu msDS-Konsystencyguid w lokalnej usłudze Active Directory. Po zapełnienia atrybutu msDS-Konsystencyguid usługi Azure AD Connect następnie eksportuje obiekt do usługi Azure AD.
    
 **Uwaga:** Po zaimportowaniu lokalnego obiektu usługi AD do programu Azure AD Connect (to jest importowane do przestrzeni łącznika usługi AD i rzutowane na Metaverse), nie można zmienić jego wartość sourceAnchor już. Aby określić wartość sourceAnchor dla danego obiektu AD lokalnego, należy skonfigurować jego atrybut msDS-Konsystencyguid przed zaimportowaniem do programu Azure AD Connect. 
  
Aby uzyskać więcej informacji na temat SourceAnchor i Konsystencyguid, odnoszą się do następującego: [Azure AD Connect: pojęcia projektowe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  


---
title: ConsistencyGuid / sourceAnchor zachowanie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659601"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="43bfb-102">ConsistencyGuid / sourceAnchor zachowanie</span><span class="sxs-lookup"><span data-stu-id="43bfb-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="43bfb-p101">Azure AD Connect (wersja 1.1.524.0 i po) teraz ułatwia korzystanie z msDS-ConsistencyGuid jako atrybut sourceAnchor. Podczas korzystania z tej funkcji Azure AD Połącz automatycznie konfiguruje reguły synchronizacji:</span><span class="sxs-lookup"><span data-stu-id="43bfb-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="43bfb-p102">Użyj msDS-ConsistencyGuid jako atrybut sourceAnchor dla obiektów użytkowników. ObjectGUID jest używany dla innych typów obiektów.</span><span class="sxs-lookup"><span data-stu-id="43bfb-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="43bfb-p103">Dla danego lokalnego użytkownika AD obiektu, którego atrybut msDS-ConsistencyGuid nie jest wypełniona, Azure pisze Połącz AD jego wartość objectGUID z powrotem do atrybutu msDS-ConsistencyGuid w usłudze Active Directory w lokalnym. Po jest wypełniane atrybut msDS-ConsistencyGuid, Azure Połącz AD następnie eksportuje obiekt Azure AD.</span><span class="sxs-lookup"><span data-stu-id="43bfb-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="43bfb-p104">**Uwaga:** Raz lokalnego obiektu AD jest importowany do Azure Połącz AD (czyli przywożone do przestrzeni łączników AD i przewidywane do obiektu Metaverse), nie można już zmienić jego wartość sourceAnchor. Aby określić wartość sourceAnchor dla biorąc pod uwagę lokalnej AD obiektów, zanim to zostanie zaimportowane do Azure Połącz AD skonfigurować jego atrybut msDS-ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="43bfb-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="43bfb-111">Aby uzyskać więcej informacji dotyczących SourceAnchor i ConsistencyGuid, odnoszą się do następujących: [Azure AD Connect: koncepcje projektowe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="43bfb-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  


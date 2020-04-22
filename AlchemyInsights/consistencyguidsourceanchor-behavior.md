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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="e98fd-102">ConsistencyGuid / sourceAchor zachowanie</span><span class="sxs-lookup"><span data-stu-id="e98fd-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="e98fd-103">Usługa Azure AD Connect (wersja 1.1.524.0 i później) ułatwia teraz korzystanie z msDS-ConsistencyGuid jako sourceAnchor atrybut.</span><span class="sxs-lookup"><span data-stu-id="e98fd-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="e98fd-104">Korzystając z tej funkcji, usługa Azure AD Connect automatycznie konfiguruje reguły synchronizacji na:</span><span class="sxs-lookup"><span data-stu-id="e98fd-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="e98fd-105">Użyj msDS-ConsistencyGuid jako sourceAnchor atrybut dla user obiektów.</span><span class="sxs-lookup"><span data-stu-id="e98fd-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="e98fd-106">ObjectGUID jest używany dla innych typów obiektów.</span><span class="sxs-lookup"><span data-stu-id="e98fd-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="e98fd-107">Dla każdego danego lokalnego obiektu użytkownika usługi AD, którego atrybut msDS-ConsistencyGuid nie jest wypełniony, usługa Azure AD Connect zapisuje swoją wartość objectGUID z powrotem do atrybutu msDS-ConsistencyGuid w lokalnej usłudze Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e98fd-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="e98fd-108">Po wypełnieniu atrybutu msDS-ConsistencyGuid usługa Azure AD Connect eksportuje obiekt do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e98fd-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="e98fd-109">**Uwaga:** Po zaimportowaniu lokalnego obiektu usługi AD do usługi Azure AD Connect (czyli zaimportowane do obszaru łącznika usługi AD i rzutowane do metaverse), nie można już zmienić jego sourceAnchor wartość.</span><span class="sxs-lookup"><span data-stu-id="e98fd-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="e98fd-110">Aby określić wartość sourceAnchor dla danego lokalnego obiektu USŁUGI AD, skonfiguruj jego atrybut msDS-ConsistencyGuid przed zaimportowaniem do usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e98fd-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="e98fd-111">Aby uzyskać więcej informacji na temat SourceAnchor i ConsistencyGuid, zobacz następujące: [Azure AD Connect: Pojęcia projektowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="e98fd-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  


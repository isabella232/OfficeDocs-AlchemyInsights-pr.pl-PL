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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="b3496-102">Zachowanie Konsystencyguid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="b3496-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="b3496-103">Azure AD Connect (wersja 1.1.524.0 i After) teraz ułatwia korzystanie z msDS-Konsystencyguid jako atrybut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="b3496-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="b3496-104">Korzystając z tej funkcji, program Azure AD Connect automatycznie konfiguruje reguły synchronizacji do:</span><span class="sxs-lookup"><span data-stu-id="b3496-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="b3496-105">Użyj msDS-Konsystencyguid jako atrybut sourceAnchor dla obiektów użytkownika.</span><span class="sxs-lookup"><span data-stu-id="b3496-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="b3496-106">ObjectGUID jest używany dla innych typów obiektów.</span><span class="sxs-lookup"><span data-stu-id="b3496-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="b3496-107">Dla dowolnego danego obiektu użytkownika AD lokalnego, którego atrybut msDS-Konsystencyguid nie jest wypełniona, program Azure AD Connect zapisuje jego wartość objectGUID z powrotem do atrybutu msDS-Konsystencyguid w lokalnej usłudze Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b3496-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="b3496-108">Po zapełnienia atrybutu msDS-Konsystencyguid usługi Azure AD Connect następnie eksportuje obiekt do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b3496-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="b3496-109">**Uwaga:** Po zaimportowaniu lokalnego obiektu usługi AD do programu Azure AD Connect (to jest importowane do przestrzeni łącznika usługi AD i rzutowane na Metaverse), nie można zmienić jego wartość sourceAnchor już.</span><span class="sxs-lookup"><span data-stu-id="b3496-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="b3496-110">Aby określić wartość sourceAnchor dla danego obiektu AD lokalnego, należy skonfigurować jego atrybut msDS-Konsystencyguid przed zaimportowaniem do programu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b3496-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="b3496-111">Aby uzyskać więcej informacji na temat SourceAnchor i Konsystencyguid, odnoszą się do następującego: [Azure AD Connect: pojęcia projektowe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="b3496-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  


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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="9bf4f-102">ConsistencyGuid/sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="9bf4f-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="9bf4f-103">Program Azure AD Connect (wersja 1.1.524.0 i po) teraz ułatwia użycie atrybutu msDS-ConsistencyGuid jako atrybutu sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="9bf4f-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="9bf4f-104">Podczas korzystania z tej funkcji program Azure AD Connect automatycznie konfiguruje reguły synchronizacji do:</span><span class="sxs-lookup"><span data-stu-id="9bf4f-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="9bf4f-105">Użyj atrybutu msDS-ConsistencyGuid jako atrybutu sourceAnchor dla obiektów User.</span><span class="sxs-lookup"><span data-stu-id="9bf4f-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="9bf4f-106">Identyfikator OBJECTGUID jest używany w przypadku innych typów obiektów.</span><span class="sxs-lookup"><span data-stu-id="9bf4f-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="9bf4f-107">W przypadku dowolnego lokalnego obiektu użytkownika usługi AD, którego atrybut msDS-ConsistencyGuid nie jest wypełniony, program Azure AD Connect zapisuje wartość objectGUID z powrotem w atrybutu msDS-ConsistencyGuid w lokalnej usłudze Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9bf4f-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="9bf4f-108">Po wypełnieniu atrybutu msDS-ConsistencyGuid program Azure AD Connect eksportuje obiekt do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9bf4f-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="9bf4f-109">**Uwaga:** Po zaimportowaniu lokalnego obiektu usługi AD do programu Azure AD Connect (czyli zaimportowania do obszaru łącznika usługi AD i wyeksportowanego do obiektu Metaverse) nie można już zmienić jego wartości sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="9bf4f-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="9bf4f-110">Aby określić wartość sourceAnchor dla danego lokalnego obiektu usługi AD, skonfiguruj jej atrybut msDS-ConsistencyGuid przed zaimportowaniu do programu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9bf4f-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="9bf4f-111">Aby uzyskać więcej informacji na temat sourceAnchor i ConsistencyGuid, zobacz następujące informacje: [Azure AD Connect: koncepcje projektowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="9bf4f-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  


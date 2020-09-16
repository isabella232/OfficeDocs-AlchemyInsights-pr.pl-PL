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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="d7687-102">Zachowanie ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="d7687-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="d7687-103">Usługa Azure AD Connect (wersja 1.1.524.0 i późniejsza) ułatwia korzystanie z msDS-ConsistencyGuid jako atrybutu sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="d7687-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="d7687-104">W przypadku korzystania z tej funkcji usługa Azure AD Connect automatycznie konfiguruje reguły synchronizacji:</span><span class="sxs-lookup"><span data-stu-id="d7687-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="d7687-105">Użyj msDS-ConsistencyGuid jako atrybutu sourceAnchor dla obiektów użytkowników.</span><span class="sxs-lookup"><span data-stu-id="d7687-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="d7687-106">ObjectGUID jest używana w przypadku innych typów obiektów.</span><span class="sxs-lookup"><span data-stu-id="d7687-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="d7687-107">W przypadku dowolnego lokalnego obiektu użytkownika usługi AD, którego atrybut msDS-ConsistencyGuid nie jest wypełniony, usługa Azure AD Connect zapisuje swoją wartość objectGUID z powrotem w atrybucie msDS-ConsistencyGuid w lokalnej usłudze Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d7687-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="d7687-108">Po wypełnieniu atrybutu msDS-ConsistencyGuid, usługa Azure AD Connect następnie eksportuje obiekt do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d7687-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="d7687-109">**Uwaga:** Po zaimportowaniu lokalnego obiektu usługi AD do usługi Azure AD Connect (czyli zaimportowaniu go do przestrzeni łącznika usług AD w celu wydzielenia go na element Metaverse) nie można już zmienić jego wartości sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="d7687-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="d7687-110">Aby określić wartość sourceAnchor dla określonego lokalnego obiektu usługi AD, skonfiguruj swój atrybut msDS-ConsistencyGuid przed zaimportowaniem go do usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d7687-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="d7687-111">Aby uzyskać więcej informacji na temat SourceAnchor i ConsistencyGuid, zapoznaj się z następującymi elementami: [Azure AD Connect: koncepcje dotyczące projektowania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="d7687-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  


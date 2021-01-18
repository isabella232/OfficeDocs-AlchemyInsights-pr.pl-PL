---
title: Synchronizacja usługi domeny
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885568"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="ad327-102">Synchronizacja usługi domeny</span><span class="sxs-lookup"><span data-stu-id="ad327-102">Domain service synchronization</span></span>

<span data-ttu-id="ad327-103">Obiekty i poświadczenia w domenie zarządzanej usługi Azure Active Directory (AD DS) mogą być tworzone lokalnie w domenie lub zsynchronizowane z dzierżawy usługi Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ad327-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="ad327-104">Po pierwszym wdrożeniu usług Azure AD DS jest konfigurowana automatyczna synchronizacja jednokierunkowa, aby można było zreplikować obiekty z usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ad327-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="ad327-105">Ta Synchronizacja jednokierunkowa nadal działa w tle, aby zapewnić aktualność domeny zarządzanej usługi Azure AD DS przy użyciu jakichkolwiek zmian z usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ad327-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="ad327-106">W usłudze Azure AD DS nie ma żadnej synchronizacji z powrotem do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ad327-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="ad327-107">Aby uzyskać więcej szczegółowych informacji na temat synchronizacji usługi domenowe w usłudze Azure Active Directory, zobacz [synchronizowanie usługi domeny](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="ad327-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 

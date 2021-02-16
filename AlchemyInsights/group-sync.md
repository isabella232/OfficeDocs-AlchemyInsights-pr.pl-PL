---
title: Synchronizacja grup
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256790"
---
# <a name="group-sync"></a><span data-ttu-id="04e86-102">Synchronizacja grup</span><span class="sxs-lookup"><span data-stu-id="04e86-102">Group sync</span></span>

<span data-ttu-id="04e86-103">Ten artykuł zawiera wskazówki dotyczące synchronizacji grup.</span><span class="sxs-lookup"><span data-stu-id="04e86-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="04e86-104">Jeśli administrator globalny lub właściciel grupy nie może modyfikować właściwości grupy, dodawać członków ani przypisywać właścicieli w portalu Azure Portal, upewnij się, że źródłem uprawnień grupy jest usługa Azure Active Directory (Azure AD) dla administratora globalnego lub właściciela grupy w celu zmodyfikowania grupy.</span><span class="sxs-lookup"><span data-stu-id="04e86-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="04e86-105">Przed podjęciem próby usunięcia zsynchronizowanej grupy w [](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) usłudze Azure AD upewnij się, że usunięto wszystkie przypisane licencje, aby uniknąć błędów.</span><span class="sxs-lookup"><span data-stu-id="04e86-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="04e86-106">Aby dowiedzieć się, jak synchronizować użytkowników, grupy i kontakty, zobacz narzędzie [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)i postępuj zgodnie z synchronizować lokalną grupę z platformą Azure za pomocą programu Azure AD [Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) w celu synchronizowania grup w ramach programu AD Connect.</span><span class="sxs-lookup"><span data-stu-id="04e86-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="04e86-107">Aby rozwiązać typowe błędy podczas [synchronizacji,](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) postępuj zgodnie z tym przewodnikiem rozwiązywania problemów podczas synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="04e86-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>


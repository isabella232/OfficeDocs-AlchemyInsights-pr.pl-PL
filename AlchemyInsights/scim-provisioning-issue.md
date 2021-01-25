---
title: SCIM z obsługą administracyjną
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949943"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="5e5b5-102">SCIM z obsługą administracyjną</span><span class="sxs-lookup"><span data-stu-id="5e5b5-102">SCIM provisioning issue</span></span>

<span data-ttu-id="5e5b5-103">Automatyczne zastrzeganie odnosi się do tworzenia tożsamości użytkowników i ról w aplikacjach w chmurze, do których mają dostęp użytkownicy.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="5e5b5-104">Ponadto, oprócz tworzenia tożsamości użytkowników, Automatyczna obsługa administracyjna obejmuje konserwację i usuwanie tożsamości użytkowników jako stan lub zmianę ról.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="5e5b5-105">Przed rozpoczęciem wdrażania możesz sprawdzić, jak działa [zainicjowanie obsługi](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) administracyjnej, aby dowiedzieć się, jak działa usługa Azure Active Directory (AD), i uzyskać zalecenia dotyczące konfiguracji.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="5e5b5-106">Jako programista aplikacji możesz korzystać z interfejsu API zarządzania użytkownikami (SCIM), aby włączyć automatyczną obsługę administracyjną użytkowników i grup między aplikacją a usługą Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="5e5b5-107">[Punkt końcowy tworzenia scim i Konfigurowanie inicjowania obsługi użytkowników za pomocą artykułu Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) zawiera opis sposobu tworzenia punktu końcowego scim i zintegrowania go z usługą udostępniania usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5e5b5-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>




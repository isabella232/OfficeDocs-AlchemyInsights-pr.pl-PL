---
title: Mapowanie atrybutów obsługi użytkowników
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
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949891"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="c9ba8-102">Mapowanie atrybutów obsługi użytkowników</span><span class="sxs-lookup"><span data-stu-id="c9ba8-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="c9ba8-103">Aby rozwiązać problemy z mapowaniem znanych atrybutów, zobacz [Mapowanie atrybutów](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="c9ba8-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="c9ba8-104">Usługa Microsoft Azure Active Directory (AD) udostępnia obsługę administracyjną użytkowników aplikacji SaaS, takich jak usługi Salesforce, usługi G Suite i inne firmy.</span><span class="sxs-lookup"><span data-stu-id="c9ba8-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="c9ba8-105">Jeśli włączysz obsługę administracyjną dla aplikacji SaaS innej firmy, usługa Azure Portal będzie kontrolować jej wartości atrybutów za pośrednictwem mapowań atrybutów.</span><span class="sxs-lookup"><span data-stu-id="c9ba8-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="c9ba8-106">Aby dowiedzieć się, jak dostosować domyślne mapowania atrybutów, zobacz [Dostosowywanie mapowania atrybutów inicjowania obsługi użytkowników dla aplikacji SaaS w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="c9ba8-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="c9ba8-107">Aby dowiedzieć się więcej o inicjowaniu obsługi użytkowników aplikacji SaaS, zobacz [co to jest zautomatyzowane Inicjowanie obsługi użytkowników aplikacji SaaS w usłudze Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="c9ba8-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="c9ba8-108">Podczas dostosowywania mapowania atrybutów do inicjowania obsługi użytkowników może się okazać, że atrybut, który chcesz zmapować, nie jest wyświetlany na liście atrybutów źródłowych.</span><span class="sxs-lookup"><span data-stu-id="c9ba8-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="c9ba8-109">Po [zsynchronizowaniu atrybutu z lokalnej usługi Active Directory z usługą Azure AD w celu udostępnienia go do](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) artykułu z aplikacją jest widoczny sposób dodawania brakującego atrybutu przez zsynchronizowanie go z lokalnej usługi AD z usługą Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c9ba8-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>

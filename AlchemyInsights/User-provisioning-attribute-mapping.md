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
# <a name="user-provisioning-attribute-mapping"></a>Mapowanie atrybutów obsługi użytkowników

1. Aby rozwiązać problemy z mapowaniem znanych atrybutów, zobacz [Mapowanie atrybutów](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Usługa Microsoft Azure Active Directory (AD) udostępnia obsługę administracyjną użytkowników aplikacji SaaS, takich jak usługi Salesforce, usługi G Suite i inne firmy. Jeśli włączysz obsługę administracyjną dla aplikacji SaaS innej firmy, usługa Azure Portal będzie kontrolować jej wartości atrybutów za pośrednictwem mapowań atrybutów. Aby dowiedzieć się, jak dostosować domyślne mapowania atrybutów, zobacz [Dostosowywanie mapowania atrybutów inicjowania obsługi użytkowników dla aplikacji SaaS w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Aby dowiedzieć się więcej o inicjowaniu obsługi użytkowników aplikacji SaaS, zobacz [co to jest zautomatyzowane Inicjowanie obsługi użytkowników aplikacji SaaS w usłudze Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Podczas dostosowywania mapowania atrybutów do inicjowania obsługi użytkowników może się okazać, że atrybut, który chcesz zmapować, nie jest wyświetlany na liście atrybutów źródłowych. Po [zsynchronizowaniu atrybutu z lokalnej usługi Active Directory z usługą Azure AD w celu udostępnienia go do](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) artykułu z aplikacją jest widoczny sposób dodawania brakującego atrybutu przez zsynchronizowanie go z lokalnej usługi AD z usługą Azure AD.

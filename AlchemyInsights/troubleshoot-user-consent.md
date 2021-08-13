---
title: Rozwiązywanie problemów ze zgodą użytkownika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007908"
---
# <a name="troubleshoot-user-consent"></a>Rozwiązywanie problemów ze zgodą użytkownika

1. Sposób wyrażania zgody przez użytkowników końcowych na aplikacje można skonfigurować za pośrednictwem portalu Azure Portal lub programu PowerShell. Aby [uzyskać więcej informacji, zobacz](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) Ustawienia zgody użytkownika.
1. Administrator może również użyć interfejsu API microsoft [Graph, aby](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) udzielić zgody na delegowane uprawnienia w imieniu jednego użytkownika. Aby uzyskać więcej informacji, zobacz [Uzyskiwanie dostępu w imieniu użytkownika.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Błędy zgody użytkownika:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)w tym artykule omówiono błędy, które mogą wystąpić podczas procesu wyrażania zgody na aplikację. Jeśli chcesz rozwiązać problem z nieoczekiwanymi monitami o zgodę, które nie zawierają komunikatów o błędach, zobacz Scenariusze uwierzytelniania [dla usługi Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
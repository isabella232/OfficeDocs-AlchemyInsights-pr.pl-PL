---
title: Rozwiązywanie problemów z zgodą użytkownika
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901634"
---
# <a name="troubleshoot-user-consent"></a>Rozwiązywanie problemów z zgodą użytkownika

1. Możesz skonfigurować sposób udzielania użytkownikom końcowym zgody na aplikacje za pośrednictwem witryny Azure Portal lub programu PowerShell. Aby uzyskać więcej informacji, zobacz [Ustawienia zgody użytkownika](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .
1. Administrator może również skorzystać z [interfejsu API programu Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) , aby udzielić zgody na delegowane uprawnienia w imieniu jednego użytkownika. Aby uzyskać więcej informacji, zobacz [Uzyskiwanie dostępu do programu Access w imieniu użytkownika](https://docs.microsoft.com/graph/auth-v2-user).
1. [Błędy zgody użytkownika](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): w tym artykule omówiono błędy, które mogą wystąpić podczas procesu wyrażania zgody na aplikację. W przypadku rozwiązywania problemów z nieoczekiwanymi monitami o zgodzie, które nie zawierają żadnych komunikatów o błędach, zobacz [scenariusze uwierzytelniania usługi Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
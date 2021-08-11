---
title: Konfiguracja serwera proxy aplikacji
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951575"
---
# <a name="app-proxy-configuration"></a>Konfiguracja serwera proxy aplikacji

1. Aby dowiedzieć się, jak skonfigurować aplikację proxy aplikacji w usłudze Azure AD w celu udostępnienia aplikacji lokalnych w chmurze, zobacz Jak skonfigurować [aplikację application proxy.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. Logowanie jednokrotne umożliwia użytkownikom uzyskiwanie dostępu do aplikacji bez uwierzytelniania wielokrotnie. Umożliwia on pojedyncze uwierzytelnianie w chmurze, na Azure Active Directory, oraz pozwala usłudze lub łącznikowi na personifikacja użytkownika, co pozwoli ukończyć wszystkie dodatkowe wyzwania związane z uwierzytelnianiem z aplikacji. Aby dowiedzieć się więcej, zobacz [Jak skonfigurować logowanie jednorazowe do aplikacji proxy.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Ten [artykuł umożliwia rozwiązywanie typowych](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) problemów występujących u innych podczas tworzenia nowej aplikacji aplikacji proxy.
4. Jeśli masz problem z skonfigurowaniem uwierzytelniania w trybie back-end dla aplikacji, może być konieczne rozwiązanie problemu z konfiguracją delegowania ograniczonego protokołu [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) dla serwera proxy aplikacji lub postępuj zgodnie ze wskazówkami na temat konfigurowania aplikacji przy użyciu programu [PingAccess,](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) aby rozwiązać ten problem.

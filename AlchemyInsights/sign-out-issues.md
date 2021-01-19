---
title: Problemy z wylogowaniem się
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901306"
---
# <a name="sign-out-issues"></a><span data-ttu-id="fd92b-102">Problemy z wylogowaniem się</span><span class="sxs-lookup"><span data-stu-id="fd92b-102">Sign-out issues</span></span>

<span data-ttu-id="fd92b-103">Aby wyeliminować problemy związane z wylogowaniem się, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="fd92b-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="fd92b-104">Jeśli użytkownik jest zalogowany lub odbierał aplikacje, należy postępować zgodnie z instrukcjami zawartymi w artykułach [Konfigurowanie zarządzania sesjami uwierzytelniania za pomocą dostępu warunkowego](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) lub [konfigurowania okresów ważności tokenów na platformie Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="fd92b-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="fd92b-105">Większość innych błędów logowania lub problemów można rozwiązać przez Rozwiązywanie problemów z integracją usługi Azure Active Directory (Azure AD) z określoną aplikacją.</span><span class="sxs-lookup"><span data-stu-id="fd92b-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="fd92b-106">Wskazówki dotyczące konkretnej integracji można znaleźć, przechodząc do tego [zestawu samouczków dotyczących integrowania aplikacji z usługą Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), w tym:</span><span class="sxs-lookup"><span data-stu-id="fd92b-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="fd92b-107">Samouczki aplikacji SaaS</span><span class="sxs-lookup"><span data-stu-id="fd92b-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="fd92b-108">Samouczki rejestracji jednokrotnej</span><span class="sxs-lookup"><span data-stu-id="fd92b-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="fd92b-109">Samouczki użytkowników</span><span class="sxs-lookup"><span data-stu-id="fd92b-109">User-provisioning tutorials</span></span>
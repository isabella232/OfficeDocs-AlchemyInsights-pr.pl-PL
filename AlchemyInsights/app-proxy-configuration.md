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
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885523"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="6f832-102">Konfiguracja serwera proxy aplikacji</span><span class="sxs-lookup"><span data-stu-id="6f832-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="6f832-103">Aby dowiedzieć się, jak skonfigurować aplikację serwera proxy aplikacji w usłudze Azure AD, aby uwidocznić aplikacje lokalne w chmurze, zobacz [jak skonfigurować aplikację serwera proxy aplikacji](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="6f832-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="6f832-104">Logowanie jednokrotne (SSO) umożliwia użytkownikom uzyskiwanie dostępu do aplikacji bez konieczności wielokrotnego uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="6f832-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="6f832-105">Umożliwia pojedyncze uwierzytelnianie w chmurze, w usłudze Azure Active Directory, oraz umożliwia usłudze lub łącznikowi personifikowanie użytkownika w celu wykonania dodatkowych wyzwań uwierzytelniania w aplikacji.</span><span class="sxs-lookup"><span data-stu-id="6f832-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="6f832-106">Aby dowiedzieć się więcej, zobacz Konfigurowanie rejestracji jednokrotnej [w aplikacji proxy aplikacji](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="6f832-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="6f832-107">[Ten artykuł](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) umożliwia rozwiązywanie typowych problemów z użytkownikami podczas tworzenia nowej aplikacji serwera proxy aplikacji.</span><span class="sxs-lookup"><span data-stu-id="6f832-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="6f832-108">Jeśli masz problem z konfigurowaniem uwierzytelniania zaplecza w aplikacji, może być konieczne [rozwiązanie ograniczeń dotyczących konfiguracji delegowania ograniczonego do protokołu Kerberos dla serwera proxy aplikacji](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) lub postępuj zgodnie z instrukcjami dotyczącymi [konfigurowania aplikacji przy użyciu PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) , aby rozwiązać ten problem.</span><span class="sxs-lookup"><span data-stu-id="6f832-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>

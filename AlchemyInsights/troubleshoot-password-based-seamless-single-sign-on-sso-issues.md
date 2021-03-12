---
title: Rozwiązywanie problemów z bezproblemowym logowaniem jednokrotnym opartym na hasłach
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714882"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="67d40-102">Rozwiązywanie problemów z bezproblemowym logowaniem jednokrotnym opartym na hasłach</span><span class="sxs-lookup"><span data-stu-id="67d40-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="67d40-103">Aby poznać podstawy logowania jednokrotnego opartego na hasłach, zobacz uwierzytelnianie oparte na hasłach za [pomocą usługi Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="67d40-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="67d40-104">**Konfigurowanie logowania jednokrotnego opartego na hasłach**</span><span class="sxs-lookup"><span data-stu-id="67d40-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="67d40-105">[Konfigurowanie logowania jednokrotnego opartego](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) na hasłach — w tym artykule opisano szczegółowo opcję logowania jednokrotnego opartą na hasłach.</span><span class="sxs-lookup"><span data-stu-id="67d40-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="67d40-106">Jeśli dodawania aplikacji wymaga konfiguracji niestandardowej i musisz używać logowania jednokrotnego opartego na hasłach, ten artykuł jest dla Ciebie.</span><span class="sxs-lookup"><span data-stu-id="67d40-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="67d40-107">[Konfigurowanie logowania pojedynczego opartego](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) na hasłach w aplikacjach wykonuj — serwer proxy aplikacji obsługuje kilka trybów logowania pojedynczego.</span><span class="sxs-lookup"><span data-stu-id="67d40-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="67d40-108">Logowanie oparte na hasłach jest przeznaczone dla aplikacji, które używają kombinacji nazwy użytkownika i hasła do uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="67d40-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="67d40-109">Podczas konfigurowania logowania opartego na hasłach dla aplikacji użytkownicy muszą zalogować się do aplikacji lokalnej jeden raz.</span><span class="sxs-lookup"><span data-stu-id="67d40-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="67d40-110">Następnie usługa Azure Active Directory przechowuje informacje logowania i automatycznie udostępnia je aplikacji, gdy użytkownicy uzyskają do nich dostęp zdalnie.</span><span class="sxs-lookup"><span data-stu-id="67d40-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="67d40-111">Aplikacja powinna już zostać opublikowana i przetestowana przy użyciu serwera proxy aplikacji.</span><span class="sxs-lookup"><span data-stu-id="67d40-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="67d40-112">Jeśli nie, wykonaj czynności opisane w tece Publikowanie aplikacji przy użyciu serwera proxy aplikacji usługi [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) a następnie kontynuuj konfigurację logowania jednokrotnego opartego na hasłach dla aplikacji w wersji wstępnej.</span><span class="sxs-lookup"><span data-stu-id="67d40-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="67d40-113">Aby rozwiązać problemy z logowaniem jednokrotnym opartym na hasłach, zobacz Rozwiązywanie problemów z logowaniem jednokrotnym opartym [na hasłach w usłudze Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="67d40-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>

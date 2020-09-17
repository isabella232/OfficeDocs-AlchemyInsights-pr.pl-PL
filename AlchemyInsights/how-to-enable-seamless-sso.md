---
title: Jak włączyć bezproblemowe logowanie jednokrotne
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780537"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="37b14-102">Jak włączyć bezproblemowe logowanie jednokrotne</span><span class="sxs-lookup"><span data-stu-id="37b14-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="37b14-103">Możliwość bezproblemowej rejestracji jednokrotnej przy użyciu [usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="37b14-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="37b14-104">Jeśli wykonujesz nową instalację usługi Azure AD Connect, wybierz [niestandardową ścieżkę instalacji](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="37b14-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="37b14-105">Na stronie **logowania użytkownika** wybierz opcję **Włącz logowanie** jednokrotne.</span><span class="sxs-lookup"><span data-stu-id="37b14-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="37b14-106">Aby sprawdzić, czy program SSO jest poprawnie włączony:</span><span class="sxs-lookup"><span data-stu-id="37b14-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="37b14-107">Zaloguj się do [Centrum administracyjnego usługi Azure Active Directory](https://aad.portal.azure.com) jako Administrator globalny.</span><span class="sxs-lookup"><span data-stu-id="37b14-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="37b14-108">Wybierz pozycję **Azure Active Directory** w okienku po lewej stronie.</span><span class="sxs-lookup"><span data-stu-id="37b14-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="37b14-109">Upewnij się, że jest **włączone**łatwe logowanie jednokrotne.</span><span class="sxs-lookup"><span data-stu-id="37b14-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="37b14-110">Aby dowiedzieć się więcej, zobacz bezproblemowa Logowanie jednokrotne [w usłudze Azure Active Directory: Szybki Start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="37b14-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  
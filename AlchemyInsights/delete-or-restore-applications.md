---
title: Usuwanie lub przywracanie aplikacji
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014906"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="6bd1d-102">Usuwanie lub przywracanie aplikacji</span><span class="sxs-lookup"><span data-stu-id="6bd1d-102">Delete or restore applications</span></span>

<span data-ttu-id="6bd1d-103">**Aby usunąć aplikację z dzierżawy usługi Azure AD**:</span><span class="sxs-lookup"><span data-stu-id="6bd1d-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="6bd1d-104">W **portalu usługi Azure AD** wybierz pozycję **aplikacje dla przedsiębiorstw**.</span><span class="sxs-lookup"><span data-stu-id="6bd1d-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="6bd1d-105">Następnie Znajdź i zaznacz aplikację, którą chcesz usunąć.</span><span class="sxs-lookup"><span data-stu-id="6bd1d-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="6bd1d-106">W sekcji **Zarządzanie** w okienku po lewej stronie wybierz pozycję **Właściwości**.</span><span class="sxs-lookup"><span data-stu-id="6bd1d-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="6bd1d-107">Wybierz pozycję **Usuń**, a następnie wybierz pozycję **tak** , aby potwierdzić, że chcesz usunąć aplikację z dzierżawy usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6bd1d-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="6bd1d-108">Aby uzyskać więcej informacji na temat usuwania aplikacji, zobacz [Szybki Start: Usuwanie aplikacji z dzierżawy usługi Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="6bd1d-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="6bd1d-109">W programie PowerShell polecenie cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) usuwa konfiguracje serwera proxy aplikacji z określonej aplikacji w usłudze Azure Active Directory i może całkowicie usunąć aplikację, jeśli jest określona.</span><span class="sxs-lookup"><span data-stu-id="6bd1d-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="6bd1d-110">**Usuniętą aplikację można przywrócić** przy użyciu programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6bd1d-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="6bd1d-111">Po zidentyfikowaniu aplikacji, którą chcesz przywrócić, możesz ją przywrócić przy użyciu polecenia [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="6bd1d-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>

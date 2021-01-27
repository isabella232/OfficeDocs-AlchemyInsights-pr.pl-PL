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
# <a name="delete-or-restore-applications"></a>Usuwanie lub przywracanie aplikacji

**Aby usunąć aplikację z dzierżawy usługi Azure AD**:

1. W **portalu usługi Azure AD** wybierz pozycję **aplikacje dla przedsiębiorstw**. Następnie Znajdź i zaznacz aplikację, którą chcesz usunąć.
2. W sekcji **Zarządzanie** w okienku po lewej stronie wybierz pozycję **Właściwości**.
3. Wybierz pozycję **Usuń**, a następnie wybierz pozycję **tak** , aby potwierdzić, że chcesz usunąć aplikację z dzierżawy usługi Azure AD.

Aby uzyskać więcej informacji na temat usuwania aplikacji, zobacz [Szybki Start: Usuwanie aplikacji z dzierżawy usługi Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

W programie PowerShell polecenie cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) usuwa konfiguracje serwera proxy aplikacji z określonej aplikacji w usłudze Azure Active Directory i może całkowicie usunąć aplikację, jeśli jest określona.

**Usuniętą aplikację można przywrócić** przy użyciu programu PowerShell. Po zidentyfikowaniu aplikacji, którą chcesz przywrócić, możesz ją przywrócić przy użyciu polecenia [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).

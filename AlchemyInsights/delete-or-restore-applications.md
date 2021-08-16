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
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102581"
---
# <a name="delete-or-restore-applications"></a>Usuwanie lub przywracanie aplikacji

**Aby usunąć aplikację z dzierżawy usługi Azure AD:**

1. W portalu **usługi Azure AD wybierz** pozycję Enterprise **aplikacji.** Następnie znajdź i zaznacz aplikację, którą chcesz usunąć.
2. W sekcji **Zarządzanie** w okienku po lewej stronie wybierz pozycję **Właściwości**.
3. Wybierz **pozycję Usuń**, a następnie wybierz pozycję **Tak,** aby potwierdzić, że chcesz usunąć aplikację z dzierżawy usługi Azure AD.

Aby uzyskać więcej informacji na temat usuwania aplikacji, zobacz Szybki start: usuwanie aplikacji z dzierżawy usługi [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

W programie PowerShell polecenie cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) usuwa konfiguracje serwera proxy aplikacji z konkretnej aplikacji w programie Azure Active Directory i może całkowicie usunąć aplikację, jeśli zostanie określona.

Usuniętą **aplikację można przywrócić za pomocą** programu PowerShell. Po zidentyfikowaniu aplikacji, którą chcesz przywrócić, możesz ją przywrócić przy użyciu [funkcji Restore-AzureADDeletedApplication.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)

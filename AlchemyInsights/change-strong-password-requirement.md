---
title: Wymaganie zmiany silnego hasła
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818478"
---
# <a name="change-strong-password-requirement"></a>Zmienianie wymagania dotyczące silnego hasła

Firma Microsoft domyślnie wymaga silnych haseł.

Za pomocą programu PowerShell możesz wyłączyć silne hasła dla konkretnych użytkowników za pomocą tych poleceń:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Aby wyłączyć silne hasła dla wszystkich użytkowników, użyj:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Więcej informacji na temat zasad dotyczących haseł](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Jak połączyć się z usługą Microsoft 365 za pomocą programu PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Więcej informacji na temat poleceń MsolUser programu PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)

---
title: Wymaganie silnego hasła zmiany
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518769"
---
# <a name="change-strong-password-requirement"></a>Wymaganie silnego hasła zmiany

Firma Microsoft wymaga silnych haseł domyślnie. 

Przy użyciu programu PowerShell, można wyłączyć silnych haseł dla określonych użytkowników, przy użyciu tego polecenia:<br>
*Cmdlettogether — UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $false*

- [Więcej informacji na temat zasad haseł](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Jak podłączyć do usługi Office 365 przy użyciu programu PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Więcej informacji na temat poleceń programu PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
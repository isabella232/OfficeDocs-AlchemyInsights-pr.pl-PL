---
title: Zmienianie wymagania silnego hasła
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
- "9000105"
- "1600"
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681882"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="b73ad-102">Zmienianie wymagania silnego hasła</span><span class="sxs-lookup"><span data-stu-id="b73ad-102">Change strong password requirement</span></span>

<span data-ttu-id="b73ad-103">Firma Microsoft domyślnie wymaga silnych haseł.</span><span class="sxs-lookup"><span data-stu-id="b73ad-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="b73ad-104">Używając programu PowerShell, możesz wyłączyć silne hasła dla określonych użytkowników za pomocą tego polecenia:</span><span class="sxs-lookup"><span data-stu-id="b73ad-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="b73ad-105">*Set-MsolUser – UserPrincipalName- <UserPrincipalName> StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="b73ad-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="b73ad-106">Więcej informacji na temat zasad haseł</span><span class="sxs-lookup"><span data-stu-id="b73ad-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="b73ad-107">Jak nawiązać połączenie z programem Microsoft 365 za pomocą programu PowerShell</span><span class="sxs-lookup"><span data-stu-id="b73ad-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="b73ad-108">Więcej informacji o poleceniach programu PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="b73ad-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)

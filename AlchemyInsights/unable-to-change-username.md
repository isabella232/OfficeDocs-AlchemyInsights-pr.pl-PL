---
title: Nie można zmienić nazwy użytkownika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440303"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="415be-102">Nie można zmienić nazwy użytkownika</span><span class="sxs-lookup"><span data-stu-id="415be-102">Unable to change UserName</span></span>

<span data-ttu-id="415be-103">W niektórych przypadkach zmiany nazwy UPN (UserPrincipalName) nie są propagowane do chmury.</span><span class="sxs-lookup"><span data-stu-id="415be-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="415be-104">Mogą pojawić się błędy sprawdzania poprawności w portalu usługi Office 365 lub nie można zmienić nazwy użytkownika lub adresu e-mail.</span><span class="sxs-lookup"><span data-stu-id="415be-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="415be-105">Aby rozwiązać ten problem, należy ręcznie ustawić userPrincipalName przy użyciu tego polecenia programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="415be-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="415be-106">**Przykład: Zmienianie nazwy użytkownika**</span><span class="sxs-lookup"><span data-stu-id="415be-106">**Example: Rename a user**</span></span>

<span data-ttu-id="415be-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="415be-107">PowerShellCopy</span></span>

<span data-ttu-id="415be-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="415be-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="415be-109">To polecenie zmienia nazwę davidc@contoso.com na davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="415be-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="415be-110">Aby uzyskać więcej informacji, zobacz [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="415be-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>
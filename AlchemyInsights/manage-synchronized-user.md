---
title: Zarządzanie zsynchronizowanym użytkownikiem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407360"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="79459-102">Nie można ustawić podstawowego adresu e-mail, zmienić atrybutów użytkownika lub usunąć/usunąć zsynchronizowanego użytkownika</span><span class="sxs-lookup"><span data-stu-id="79459-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="79459-103">Jeśli synchronizacja katalogów jest włączona w twoim środowisku, nie można zmienić niektórych atrybutów użytkownika lub obiektu za pomocą centrum administracyjnego usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="79459-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="79459-104">Aby w pełni zarządzać zsynchronizowanymi użytkownikami i wszystkimi ich atrybutami, użyj lokalnej konsoli zarządzania usługi Active Directory (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="79459-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="79459-105">Alternatywnie można zmienić poszczególnych użytkowników lub atrybuty dla zsynchronizowanych użytkowników przy użyciu programu PowerShell, takie jak pokazano w poniższych typowych przykładach:</span><span class="sxs-lookup"><span data-stu-id="79459-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`

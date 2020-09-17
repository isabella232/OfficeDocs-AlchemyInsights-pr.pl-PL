---
title: Zarządzanie synchronizowanym użytkownikiem
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
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777687"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="e14dd-102">Nie można ustawić podstawowego adresu e-mail, zmienić atrybutów użytkownika ani usunąć/usunąć synchronizowanego użytkownika</span><span class="sxs-lookup"><span data-stu-id="e14dd-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="e14dd-103">Jeśli dla danego środowiska włączono synchronizację katalogów, niektóre atrybuty użytkowników i obiektów nie mogą być zmieniane przy użyciu Centrum administracyjnego Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e14dd-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="e14dd-104">Aby w pełni zarządzać synchronizowanymi użytkownikami i wszystkimi ich atrybutami, użyj konsoli zarządzania lokalni użytkownicy i grupy usługi Active Directory (Adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="e14dd-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="e14dd-105">Możesz też zmienić poszczególnych użytkowników lub atrybuty dla synchronizowanych użytkowników przy użyciu programu PowerShell, takich jak pokazano w następujących typowych przykładach:</span><span class="sxs-lookup"><span data-stu-id="e14dd-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`

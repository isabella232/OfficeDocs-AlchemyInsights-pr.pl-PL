---
title: Zarządzanie synchronizowanych użytkowników
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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542009"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="db54e-102">Nie można ustawić podstawowy adres e-mail lub zmienić atrybuty użytkownika</span><span class="sxs-lookup"><span data-stu-id="db54e-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="db54e-103">Po włączeniu synchronizacji katalogów w danym środowisku niektórych atrybutów obiektu użytkownika lub nie można zmienić za pomocą Centrum administracyjnego usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="db54e-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="db54e-104">Aby w pełni zarządzać zsynchronizowanych użytkowników i ich atrybutów, użyj lokalną usługę active directory użytkownicy i grupy konsoli zarządzania (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="db54e-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="db54e-105">Można również zmienić poszczególnym użytkownikom lub atrybutów dla użytkowników zsynchronizowanych przy użyciu programu powershell, takich jak pokazano w tych przykładach wspólne:</span><span class="sxs-lookup"><span data-stu-id="db54e-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="db54e-106">Cmdlettogether - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="db54e-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="db54e-107">Cmdlettogether - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Użytkownika testowego" - LastName "Użytkownik"-tytuł "Menedżer"-dział "HR"</span><span class="sxs-lookup"><span data-stu-id="db54e-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="db54e-108">Usuń MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="db54e-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>
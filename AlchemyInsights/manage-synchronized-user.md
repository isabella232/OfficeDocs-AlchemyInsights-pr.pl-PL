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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380515"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="c93aa-102">Nie można ustawić podstawowy adres e-mail lub zmienić atrybuty użytkownika</span><span class="sxs-lookup"><span data-stu-id="c93aa-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="c93aa-103">Po włączeniu synchronizacji katalogów w danym środowisku niektórych atrybutów obiektu użytkownika lub nie można zmienić przy użyciu Centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="c93aa-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="c93aa-104">Aby w pełni zarządzać zsynchronizowanych użytkowników i ich atrybutów, użyj lokalną usługę active directory użytkownicy i grupy konsoli zarządzania (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="c93aa-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="c93aa-105">Można również zmienić poszczególnym użytkownikom lub atrybutów dla użytkowników zsynchronizowanych przy użyciu programu powershell, takich jak pokazano w tych przykładach wspólne:</span><span class="sxs-lookup"><span data-stu-id="c93aa-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="c93aa-106">Cmdlettogether - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="c93aa-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="c93aa-107">Cmdlettogether - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Użytkownika testowego" - LastName "Użytkownik"-tytuł "Menedżer"-dział "HR"</span><span class="sxs-lookup"><span data-stu-id="c93aa-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="c93aa-108">Usuń MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="c93aa-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>
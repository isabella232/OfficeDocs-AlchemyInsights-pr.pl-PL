---
title: Wielu użytkowników nie widzi dodatków w programie Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198237"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="f99b7-102">Wielu użytkowników nie widzi dodatków w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="f99b7-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="f99b7-103">Jeśli testujesz dodatki programu Outlook i żaden nie jest pokazywany, jako pierwszy krok rozwiązywania problemów, użyj polecenia cmdlet **Get-OrganizationConfig** PowerShell, aby wykonać kwerendę parametru _AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="f99b7-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="f99b7-104">Jeśli kwerenda zwraca wartość **False,** ustaw ten parametr na **True** przy użyciu polecenia cmdlet **Set-OrganizationConfig,** więc dodatki są wyświetlane zgodnie z oczekiwaniami.</span><span class="sxs-lookup"><span data-stu-id="f99b7-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="f99b7-105">Nie zaleca się, aby parametr _AppsForOfficeEnabled_ był ustawiony na **False**.</span><span class="sxs-lookup"><span data-stu-id="f99b7-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="f99b7-106">Wartość **False** zastępuje wszystkie powyższe ustawienia roli administracyjne i użytkownika i zapobiega aktywowaniu nowych aplikacji przez dowolnego użytkownika w organizacji.</span><span class="sxs-lookup"><span data-stu-id="f99b7-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="f99b7-107">Aby uzyskać więcej informacji, zobacz [Określanie administratorów i użytkowników, którzy mogą instalować dodatki programu Outlook i zarządzać nimi.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)</span><span class="sxs-lookup"><span data-stu-id="f99b7-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>
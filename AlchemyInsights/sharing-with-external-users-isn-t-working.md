---
title: Udostępnianie użytkownikom zewnętrznym nie działa
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767259"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="b788e-102">Rozwiązywanie problemów z udostępnianiem zawartości programu SharePoint użytkownikom zewnętrznym</span><span class="sxs-lookup"><span data-stu-id="b788e-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="b788e-103">Upewnij się, że udostępnianie zewnętrzne jest włączone w twojej organizacji:</span><span class="sxs-lookup"><span data-stu-id="b788e-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="b788e-104">Przejdź do [ &amp; strony Dodatki usług w centrum administracyjnym usługi Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i kliknij pozycję **Witryny**.</span><span class="sxs-lookup"><span data-stu-id="b788e-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="b788e-105">Upewnij się, że ustawienie jest włączone.</span><span class="sxs-lookup"><span data-stu-id="b788e-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="b788e-106">Jeśli wybrano opcję "Tylko istniejący użytkownicy zewnętrzni", upewnij się, że użytkownik zewnętrzny znajduje się na liście w centrum administracyjnym usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b788e-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="b788e-107">Upewnij się, że udostępnianie zewnętrzne jest włączone dla witryny.</span><span class="sxs-lookup"><span data-stu-id="b788e-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="b788e-108">W przypadku klasycznego zbioru witryn:</span><span class="sxs-lookup"><span data-stu-id="b788e-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="b788e-109">W nowym centrum administracyjnym programu SharePoint w lewym okienku kliknij pozycję **Witryny**.</span><span class="sxs-lookup"><span data-stu-id="b788e-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="b788e-110">Wybierz witrynę lub witryny, a na wstążce kliknij pozycję **Udostępnianie**.</span><span class="sxs-lookup"><span data-stu-id="b788e-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="b788e-111">W przypadku witryny zespołu należącej do grupy usługi Office 365 lub witryny komunikacyjnej:</span><span class="sxs-lookup"><span data-stu-id="b788e-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="b788e-112">Te nowe typy witryn mają takie samo ustawienie udostępniania jak ustawienie dla całej organizacji, chyba że ustawienie dla całej organizacji umożliwia udostępnianie plików przy użyciu łączy, które nie wymagają logowania.</span><span class="sxs-lookup"><span data-stu-id="b788e-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="b788e-113">W takim przypadku witryny umożliwiają udostępnianie nowym i istniejącym użytkownikom zewnętrznym, którzy się logują.</span><span class="sxs-lookup"><span data-stu-id="b788e-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="b788e-114">Aby zmienić ustawienie dla określonych witryn, użyj nowego centrum administracyjnego programu SharePoint lub programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b788e-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="b788e-115">[Dowiedz się więcej](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="b788e-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="b788e-116">Ustawienie udostępniania zewnętrznego dla dowolnej witryny może być bardziej restrykcyjne niż ustawienie dla całej organizacji, ale nie bardziej dopuszczalne niż ustawienie dla całej organizacji.</span><span class="sxs-lookup"><span data-stu-id="b788e-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  


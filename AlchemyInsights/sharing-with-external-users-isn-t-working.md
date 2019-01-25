---
title: Udostępnianie użytkownikom zewnętrznym nie działa
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482804"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="b890e-102">Rozwiązywanie problemów z udostępniania zawartości programu SharePoint dla użytkowników zewnętrznych</span><span class="sxs-lookup"><span data-stu-id="b890e-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="b890e-103">Upewnij się, że udostępniania zewnętrznych jest włączona dla organizacji:</span><span class="sxs-lookup"><span data-stu-id="b890e-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="b890e-104">Przejdź do [usług &amp; stronę dodatki w Centrum administracyjnym usługi Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i kliknij przycisk **witryny**.</span><span class="sxs-lookup"><span data-stu-id="b890e-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="b890e-p101">Upewnij się, że włączono ustawienie na "On". Jeśli zaznaczone jest "Tylko istniejących użytkowników zewnętrznych", upewnij się, zewnętrzne użytkownik jest wyświetlany w Centrum administracyjnym usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="b890e-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="b890e-p102">Upewnij się, udostępniania zewnętrznych włączone dla witryny. Dla zbioru witryn klasyczne:</span><span class="sxs-lookup"><span data-stu-id="b890e-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="b890e-109">W klasycznym Centrum administracyjnego programu SharePoint, w lewym okienku kliknij **zbiorów witryn**.</span><span class="sxs-lookup"><span data-stu-id="b890e-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="b890e-110">Wybierz witrynę lub witryny, a na wstążce kliknij polecenie **Udostępnianie**.</span><span class="sxs-lookup"><span data-stu-id="b890e-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="b890e-111">Dla witryny zespołu, który należy do grupy usługi Office 365, lub witryny komunikacji:</span><span class="sxs-lookup"><span data-stu-id="b890e-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="b890e-p103">Te nowe typy witryny mają sam ustawienie udostępniania ustawienie całej organizacji, chyba że ustawienie całej organizacji pozwala na udostępnianie plików przy użyciu łącza, które nie wymagają rejestrowania. W takim przypadku witryn Zezwalaj na współużytkowanie z nowych i istniejących użytkowników zewnętrznych, którzy Zaloguj się. Aby zmienić ustawienie dla określonych witryn, należy użyć nowego Centrum administracyjnego programu SharePoint (Podgląd) lub programu PowerShell. [Dowiedz się więcej](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="b890e-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="b890e-116">Ustawienia udostępniania zewnętrznych dla dowolnej witryny mogą być bardziej restrykcyjne niż ustawienia całej organizacji, ale nie bardziej liberalne niż ustawienie całej organizacji.</span><span class="sxs-lookup"><span data-stu-id="b890e-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  


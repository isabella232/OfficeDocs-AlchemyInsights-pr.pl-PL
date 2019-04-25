---
title: Udostępnianie użytkownikom zewnętrznym nie działa
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369508"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="d2171-102">Rozwiązywanie problemów z udostępniania zawartości programu SharePoint dla użytkowników zewnętrznych</span><span class="sxs-lookup"><span data-stu-id="d2171-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="d2171-103">Upewnij się, że udostępniania zewnętrznych jest włączona dla organizacji:</span><span class="sxs-lookup"><span data-stu-id="d2171-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="d2171-104">Przejdź do [usług &amp; stronę dodatki w Centrum administracyjnym usługi Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i kliknij przycisk **witryny**.</span><span class="sxs-lookup"><span data-stu-id="d2171-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="d2171-105">Upewnij się, że włączono ustawienie na "On".</span><span class="sxs-lookup"><span data-stu-id="d2171-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="d2171-106">Jeśli zaznaczone jest "Tylko istniejących użytkowników zewnętrznych", upewnij się, zewnętrzne użytkownik jest wyświetlany w Centrum administracyjnym usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d2171-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="d2171-107">Upewnij się, udostępniania zewnętrznych włączone dla witryny.</span><span class="sxs-lookup"><span data-stu-id="d2171-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="d2171-108">Dla zbioru witryn klasyczne:</span><span class="sxs-lookup"><span data-stu-id="d2171-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="d2171-109">W nowym Centrum administracji programu SharePoint, w lewym okienku kliknij przycisk **witryny**.</span><span class="sxs-lookup"><span data-stu-id="d2171-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="d2171-110">Wybierz witrynę lub witryny, a na wstążce kliknij polecenie **Udostępnianie**.</span><span class="sxs-lookup"><span data-stu-id="d2171-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="d2171-111">Dla witryny zespołu, który należy do grupy usługi Office 365, lub witryny komunikacji:</span><span class="sxs-lookup"><span data-stu-id="d2171-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="d2171-112">Te nowe typy witryny mają sam ustawienie udostępniania ustawienie całej organizacji, chyba że ustawienie całej organizacji pozwala na udostępnianie plików przy użyciu łącza, które nie wymagają rejestrowania.</span><span class="sxs-lookup"><span data-stu-id="d2171-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="d2171-113">W takim przypadku witryn Zezwalaj na współużytkowanie z nowych i istniejących użytkowników zewnętrznych, którzy Zaloguj się.</span><span class="sxs-lookup"><span data-stu-id="d2171-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="d2171-114">Aby zmienić to ustawienie dla określonych witryn, należy użyć nowego Centrum administracyjnego programu SharePoint lub programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d2171-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="d2171-115">[Dowiedz się więcej](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="d2171-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="d2171-116">Ustawienia udostępniania zewnętrznych dla dowolnej witryny mogą być bardziej restrykcyjne niż ustawienia całej organizacji, ale nie bardziej liberalne niż ustawienie całej organizacji.</span><span class="sxs-lookup"><span data-stu-id="d2171-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  


---
title: Udostępnianie użytkownikom zewnętrznym nie działa
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691585"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="6f33d-102">Rozwiązywanie problemów z udostępnianiem zawartości programu SharePoint użytkownikom zewnętrznym</span><span class="sxs-lookup"><span data-stu-id="6f33d-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="6f33d-103">Upewnij się, że funkcja udostępniania zewnętrznego jest włączona w Twojej organizacji:</span><span class="sxs-lookup"><span data-stu-id="6f33d-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="6f33d-104">Przejdź do [ &amp; strony Dodatki usług w centrum administracyjnym usługi Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a następnie kliknij pozycję **witryny**.</span><span class="sxs-lookup"><span data-stu-id="6f33d-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="6f33d-105">Upewnij się, że ustawienie jest włączone.</span><span class="sxs-lookup"><span data-stu-id="6f33d-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="6f33d-106">Jeśli jest zaznaczona pozycja "tylko istniejący użytkownik zewnętrzny", upewnij się, że użytkownik zewnętrzny jest wymieniony w centrum administracyjnym usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6f33d-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="6f33d-107">Upewnij się, że włączono udostępnianie zewnętrzne witryny.</span><span class="sxs-lookup"><span data-stu-id="6f33d-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="6f33d-108">W przypadku klasycznego zbioru witryn:</span><span class="sxs-lookup"><span data-stu-id="6f33d-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="6f33d-109">W nowym centrum administracyjnym programu SharePoint w okienku po lewej stronie kliknij pozycję **witryny**.</span><span class="sxs-lookup"><span data-stu-id="6f33d-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="6f33d-110">Wybierz witrynę lub witryny, a następnie na wstążce kliknij pozycję **udostępnianie**.</span><span class="sxs-lookup"><span data-stu-id="6f33d-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="6f33d-111">W przypadku witryny zespołu należącej do grupy programu Microsoft 365 lub witryny do komunikacji:</span><span class="sxs-lookup"><span data-stu-id="6f33d-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="6f33d-112">Te nowe typy witryn mają to samo ustawienie udostępniania, co ustawienie w całej organizacji, chyba że ustawienie całej organizacji umożliwia udostępnianie plików za pomocą linków, które nie wymagają logowania.</span><span class="sxs-lookup"><span data-stu-id="6f33d-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="6f33d-113">W tym przypadku witryny umożliwiają udostępnianie nowym i istniejącym użytkownikom zewnętrznym, którzy będą logować się.</span><span class="sxs-lookup"><span data-stu-id="6f33d-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="6f33d-114">Aby zmienić ustawienie dla określonych witryn, Użyj nowego centrum administracyjnego programu SharePoint lub programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6f33d-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="6f33d-115">[Dowiedz się więcej](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="6f33d-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="6f33d-116">Ustawienia udostępniania zewnętrznego dla dowolnej witryny mogą być bardziej restrykcyjne niż ustawienia dla całej organizacji, ale nie są one ograniczane od ustawienia dla całej organizacji.</span><span class="sxs-lookup"><span data-stu-id="6f33d-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  


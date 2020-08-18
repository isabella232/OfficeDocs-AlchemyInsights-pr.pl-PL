---
title: Tworzenie witryny programu SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786575"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="3caa4-102">Tworzenie witryny programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="3caa4-102">Create a SharePoint site</span></span>

<span data-ttu-id="3caa4-103">Tworzenie witryn i zarządzanie nimi z [aktywnych witryn](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) w centrum administracyjnym programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3caa4-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="3caa4-104">Aby uzyskać więcej informacji, zobacz [Zarządzanie witrynami w nowym centrum administracyjnym programu SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="3caa4-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="3caa4-105">Końcówk</span><span class="sxs-lookup"><span data-stu-id="3caa4-105">Tips:</span></span>

- <span data-ttu-id="3caa4-106">**Nie można** utworzyć witryny o tym samym adresie URL istniejącej witryny.</span><span class="sxs-lookup"><span data-stu-id="3caa4-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="3caa4-107">Jeśli witryna została usunięta i chcesz ponownie użyć adresu URL, usunięta witryna nadal będzie dostępna w obszarze [usunięte witryny](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="3caa4-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="3caa4-108">Aby ponownie użyć adresu URL, witryna musi zostać trwale usunięta.</span><span class="sxs-lookup"><span data-stu-id="3caa4-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="3caa4-109">Aby całkowicie usunąć witrynę za pomocą programu PowerShell, zobacz przykład polecenia cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="3caa4-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="3caa4-110">Niektóre użytkownicy mogą nie być w stanie utworzyć witryny.</span><span class="sxs-lookup"><span data-stu-id="3caa4-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="3caa4-111">[Zobacz Zarządzanie tworzeniem witryn w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="3caa4-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="3caa4-112">Możliwe, że witryna jest zablokowana w przypadku dłuższego **tworzenia** .</span><span class="sxs-lookup"><span data-stu-id="3caa4-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="3caa4-113">Jeśli od momentu pierwszego uruchomienia tego problemu minęło więcej niż 24 godziny, zarejestruj bilet pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="3caa4-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="3caa4-114">W wielu przypadkach jesteśmy już nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="3caa4-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="3caa4-115">Przekaż nam co najmniej 24 godziny na zakończenie rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="3caa4-115">Please give us at least 24 hours to complete a solution.</span></span>

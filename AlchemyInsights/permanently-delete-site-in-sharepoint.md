---
title: Trwałe usuwanie witryny w programie SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955243"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="f9d3b-102">Trwałe usuwanie witryny w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="f9d3b-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="f9d3b-103">Aby ponownie użyć adresu URL z usuniętej witryny (w celu odtworzenia witryny) lub trwale usunąć witrynę, ponieważ nie jest już używana, możesz użyć pozycji **Trwale usuń** z nowego centrum administracyjnego programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f9d3b-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="f9d3b-104">Przejdź [na stronę usuniętych witryn nowego centrum administracyjnego programu SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) i zaloguj się przy użyciu konta z uprawnieniami administratora dla organizacji.</span><span class="sxs-lookup"><span data-stu-id="f9d3b-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="f9d3b-105">W kolumnie po lewej stronie wybierz witrynę.</span><span class="sxs-lookup"><span data-stu-id="f9d3b-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="f9d3b-106">Kliknij pozycję **Trwale usuń**.</span><span class="sxs-lookup"><span data-stu-id="f9d3b-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="f9d3b-107">**Uwaga**: Nie można trwale usunąć witryn połączonych z grupami w nowym centrum administracyjnym programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f9d3b-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="f9d3b-108">Zamiast tego należy użyć polecenia [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="f9d3b-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="f9d3b-109">Aby uzyskać więcej informacji, zobacz [Trwałe usuwanie witryny](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="f9d3b-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 

---
title: Usuwanie witryny głównej programu SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815481"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="2b6cf-102">Usuwanie witryny głównej programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="2b6cf-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="2b6cf-103">Usuwanie witryny głównej programu SharePoint  **nie jest obsługiwane.**</span><span class="sxs-lookup"><span data-stu-id="2b6cf-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="2b6cf-104">Jeśli witryna główna została już usunięta, podczas próby uzyskania dostępu do witryny będzie wyświetlany błąd 404 Nie można odnaleźć pliku.</span><span class="sxs-lookup"><span data-stu-id="2b6cf-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="2b6cf-105">Aby rozwiązać problem, przywróć witrynę z [](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) nowego centrum administracyjnego programu SharePoint, przechodząc do strony Usunięte witryny, wybierz witrynę główną i kliknij pozycję Przywróć.</span><span class="sxs-lookup"><span data-stu-id="2b6cf-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="2b6cf-106">Zamiast usuwać witrynę [](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) główną, po przywróceniu witryny głównej użyj zamieniania witryny z nowego Centrum administracyjnego programu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2b6cf-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="2b6cf-107">Aby uzyskać więcej informacji, zobacz [Unowocześniowanie witryny głównej.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="2b6cf-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>
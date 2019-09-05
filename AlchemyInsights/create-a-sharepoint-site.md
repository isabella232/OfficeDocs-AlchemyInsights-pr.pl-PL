---
title: Tworzenie witryny programu SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738207"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="033a0-102">Tworzenie witryny programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="033a0-102">Create a SharePoint site</span></span>

<span data-ttu-id="033a0-103">Można wyświetlić następujące informacje dotyczące tworzenia witryny programu SharePoint:</span><span class="sxs-lookup"><span data-stu-id="033a0-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="033a0-104">[Zarządzaj witrynami w nowym centrum administracyjnym programu SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Dowiedz się więcej o opcjach tworzenia witryny, w tym o sposobie tworzenia klasycznej witryny lub witryny zespołów, która nie zawiera grupy 365 pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="033a0-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="033a0-105">[Tworzenie witryny zespołu w programie SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Dowiedz się, jak utworzyć witrynę zespołu.</span><span class="sxs-lookup"><span data-stu-id="033a0-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="033a0-106">[Tworzenie witryny komunikacji w programie SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Dowiedz się, jak utworzyć witrynę komunikacji.</span><span class="sxs-lookup"><span data-stu-id="033a0-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="033a0-107">[Zarządzaj witrynami w nowym centrum administracyjnym programu SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Dowiedz się, jak utworzyć klasyczną witrynę lub witrynę zespołu, która nie zawiera grupy 365 pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="033a0-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="033a0-108">[! Wskazówki</span><span class="sxs-lookup"><span data-stu-id="033a0-108">[!Tips]</span></span>
> - <span data-ttu-id="033a0-109">Nie można utworzyć witryny o tym samym adresie URL istniejącej witryny.</span><span class="sxs-lookup"><span data-stu-id="033a0-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="033a0-110">Jeśli usunięto witrynę i chcą ponownie użyć adresu URL, jest możliwe, że usunięte witryny nadal istnieje w obszarze **usuniętych witryn**.</span><span class="sxs-lookup"><span data-stu-id="033a0-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="033a0-111">Aby zarządzać usuniętymi witrynami, zobacz [usuwanie witryny](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="033a0-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="033a0-112">Aby całkowicie usunąć witrynę za pomocą programu PowerShell, zobacz przykład polecenia cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="033a0-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="033a0-113">Niektórzy użytkownicy mogą nie być w stanie utworzyć witryny.</span><span class="sxs-lookup"><span data-stu-id="033a0-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="033a0-114">Zobacz [Zarządzanie tworzeniem witryn w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="033a0-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="033a0-115">Jest możliwe, że witryna pojawia się zatrzymany na **Tworzenie** dłużej niż oczekiwano.</span><span class="sxs-lookup"><span data-stu-id="033a0-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="033a0-116">Jeśli minęło więcej niż 24 godziny od pierwszego zobaczyłem ten problem, należy zalogować bilet pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="033a0-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="033a0-117">W wielu przypadkach pracujemy już nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="033a0-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="033a0-118">Proszę dać nam co najmniej 24 godziny, aby zakończyć rozwiązanie.</span><span class="sxs-lookup"><span data-stu-id="033a0-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="033a0-119">Jeśli musisz utworzyć nową witrynę zespołu, która nie zawiera grupy 365 pakietu Office,</span><span class="sxs-lookup"><span data-stu-id="033a0-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 



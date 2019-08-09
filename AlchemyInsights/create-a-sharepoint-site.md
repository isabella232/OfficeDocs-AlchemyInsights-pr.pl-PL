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
ms.openlocfilehash: ad1a77b69d2d453dbd3daa304759238b329f96ba
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269926"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="af717-102">Tworzenie witryny programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="af717-102">Create a SharePoint site</span></span>

<span data-ttu-id="af717-103">Można wyświetlić następujące informacje dla informacji na temat tworzenia witryn programu SharePoint:</span><span class="sxs-lookup"><span data-stu-id="af717-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="af717-104">[Zarządzanie witrynami w Centrum administracyjnego programu SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Dowiedz się więcej o opcji tworzenia witryny, w tym sposobu tworzenia klasyczne witryny lub witryny zespołów, który nie zawiera grupę w usłudze Office 365.</span><span class="sxs-lookup"><span data-stu-id="af717-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="af717-105">[Utwórz witrynę zespołu w programie SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Dowiedz się, jak utworzyć witrynę zespołu.</span><span class="sxs-lookup"><span data-stu-id="af717-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="af717-106">[Utwórz witrynę komunikacji w dokumentacji Online programu SharePoint](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Dowiedz się, jak utworzyć witrynę komunikacji.</span><span class="sxs-lookup"><span data-stu-id="af717-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="af717-107">[Zarządzanie witrynami w Centrum administracyjnego programu SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Dowiedz się, jak utworzyć klasyczne witryny lub witryny zespołu, który nie zawiera grupę w usłudze Office 365.</span><span class="sxs-lookup"><span data-stu-id="af717-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Porady]
> - <span data-ttu-id="af717-109">Nie można utworzyć witryny z tego samego adresu URL istniejącej witryny.</span><span class="sxs-lookup"><span data-stu-id="af717-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="af717-110">Jeśli usunięte z witryny i chcą ponownie użyć adresu URL, jest możliwe, usunięte strony nadal istnieje w obszarze **witryny elementów usuniętych**.</span><span class="sxs-lookup"><span data-stu-id="af717-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="af717-111">Aby zarządzać usunięte witryn, zobacz [Usuwanie witryny](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="af717-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="af717-112">Aby całkowicie usunąć witryny przy użyciu programu Powershell, zobacz przykład polecenia cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="af717-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="af717-113">Niektórym użytkownikom nie można utworzyć lokację.</span><span class="sxs-lookup"><span data-stu-id="af717-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="af717-114">Zobacz [Tworzenie witryny Zarządzanie w dokumentacji Online programu SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="af717-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="af717-115">Jest możliwe, witryna zostanie wyświetlone zatrzymany na **Tworzenie** dłużej, niż oczekiwano.</span><span class="sxs-lookup"><span data-stu-id="af717-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="af717-116">Jeśli więcej niż 24 godziny minęło po raz pierwszy zobaczył ten problem, należy zalogować się do pomocy technicznej.</span><span class="sxs-lookup"><span data-stu-id="af717-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="af717-117">W wielu przypadkach już pracujemy nad rozwiązaniem.</span><span class="sxs-lookup"><span data-stu-id="af717-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="af717-118">Podaj co najmniej 24 godziny, aby ukończyć rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="af717-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="af717-119">Jeśli zachodzi konieczność utworzenia nowej witryny zespołu, który nie zawiera grupę usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="af717-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 



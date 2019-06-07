---
title: Dodawanie grupy do witryny programu SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758740"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="fa53a-102">Tworzenie grupy witryn połączonych w dokumentacji Online programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="fa53a-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="fa53a-103">Istnieje kilka typowych problemów napotykanych podczas tworzenia lub ponownego tworzenia grupy połączenia witryny.</span><span class="sxs-lookup"><span data-stu-id="fa53a-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="fa53a-104">Jeśli usunięto grupę i jej witryn połączonych i chcesz utworzyć inną witrynę z tego samego adresu URL, należy trwale usunąć poprzedniej witryny.</span><span class="sxs-lookup"><span data-stu-id="fa53a-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="fa53a-105">Pobierz [powłoki zarządzania SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="fa53a-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="fa53a-106">Aby uzyskać więcej informacji na temat korzystania ze środowiska powershell zobacz [Online powłoki zarządzania programu SharePoint — wprowadzenie](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="fa53a-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="fa53a-107">Usuń witrynę z witryn usunięte za pomocą polecenia cmdlet [Remove-Spodeletedsitedla](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) środowiska powershell.</span><span class="sxs-lookup"><span data-stu-id="fa53a-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="fa53a-108">Jeśli tworzysz witrynę grupy a pojawia się ostrzeżenie, że innej grupy z takiego samego aliasu już istnieje, sprawdź istniejących grup z [usługi Office 365 z Centrum administracyjnego](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="fa53a-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="fa53a-109">Aby rozwiązać ten problem, usuń istniejącą grupę, jeśli nie jest już potrzebne lub utworzyć witrynę z inny alias przydzielony.</span><span class="sxs-lookup"><span data-stu-id="fa53a-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="fa53a-110">Istnieją różne sposoby tworzenia i używania nowoczesnych grup z programem SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fa53a-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="fa53a-111">Istniejące witryny można połączyć się z grupą usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="fa53a-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="fa53a-112">Aby uzyskać więcej informacji zobacz [Łączenie grupę Office 365 przy użyciu ineterface użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="fa53a-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="fa53a-113">Aby utworzyć witrynę połączonych grup usługi Office 365, musisz utworzyć witrynę zespołu.</span><span class="sxs-lookup"><span data-stu-id="fa53a-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="fa53a-114">Aby uzyskać więcej informacji zobacz [Tworzenie witryny zespołu w programie SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="fa53a-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>


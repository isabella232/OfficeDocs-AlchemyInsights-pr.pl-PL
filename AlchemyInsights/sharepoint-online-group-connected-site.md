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
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507857"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="436dd-102">Problemy podczas tworzenia lub grupy witryn programu SharePoint Online połączony</span><span class="sxs-lookup"><span data-stu-id="436dd-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="436dd-103">Istnieje kilka typowych problemów napotykanych podczas tworzenia lub ponownego tworzenia grupy połączenia witryny.</span><span class="sxs-lookup"><span data-stu-id="436dd-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="436dd-104">Jeśli usunięto grupę i jej witryn połączonych i chcesz utworzyć inną witrynę z tego samego adresu URL, należy trwale usunąć poprzedniej witryny.</span><span class="sxs-lookup"><span data-stu-id="436dd-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="436dd-105">Pobierz [powłoki zarządzania SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="436dd-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="436dd-106">Aby uzyskać więcej informacji na temat korzystania ze środowiska powershell zobacz [Online powłoki zarządzania programu SharePoint — wprowadzenie](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="436dd-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="436dd-107">Usuń witrynę z witryn usunięte za pomocą polecenia cmdlet [Remove-Spodeletedsitedla](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) środowiska powershell.</span><span class="sxs-lookup"><span data-stu-id="436dd-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="436dd-108">Jeśli tworzysz witrynę grupy a pojawia się ostrzeżenie, że innej grupy z takiego samego aliasu już istnieje, sprawdź istniejących grup z [usługi Office 365 z Centrum administracyjnego](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="436dd-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="436dd-109">Aby rozwiązać ten problem, usuń istniejącą grupę, jeśli nie jest już potrzebne lub utworzyć witrynę z inny alias przydzielony.</span><span class="sxs-lookup"><span data-stu-id="436dd-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="436dd-110">Istnieją różne sposoby tworzenia i używania nowoczesnych grup z programem SharePoint.</span><span class="sxs-lookup"><span data-stu-id="436dd-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="436dd-111">Istniejące witryny można połączyć się z grupą usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="436dd-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="436dd-112">Aby uzyskać więcej informacji zobacz [Łączenie grupę Office 365 przy użyciu ineterface użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="436dd-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="436dd-113">Aby utworzyć witrynę połączonych grup usługi Office 365, musisz utworzyć witrynę zespołu.</span><span class="sxs-lookup"><span data-stu-id="436dd-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="436dd-114">Aby uzyskać więcej informacji zobacz [Tworzenie witryny zespołu w programie SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="436dd-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>


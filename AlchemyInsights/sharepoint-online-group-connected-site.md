---
title: Dodawanie grupy do witryny programu SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051111"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="5d0c5-102">Problemy podczas tworzenia lub grupowania połączonych witryn w programie SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5d0c5-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="5d0c5-103">Istnieje kilka typowych problemów napotkanych podczas tworzenia lub ponownego tworzenia grupy połączonej witryny.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="5d0c5-104">W przypadku usunięcia grupy i jej połączonej witryny i chęci utworzenia innej witryny z tym samym adresem URL, należy trwale usunąć poprzednią witrynę.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="5d0c5-105">Pobierz za darmo [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="5d0c5-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="5d0c5-106">Aby uzyskać więcej informacji na wprowadzenie do programu PowerShell, zobacz [wprowadzenie do programu SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="5d0c5-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="5d0c5-107">Usuń witrynę z usuniętych witryn za pomocą polecenia cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="5d0c5-108">Jeśli tworzysz grupę połączonej witryny i otrzymujesz ostrzeżenie inna grupa o tym samym aliasie już istnieje, Sprawdź istniejące grupy z [pakietu Office 365 z centrum administracyjnego](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="5d0c5-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="5d0c5-109">Aby rozwiązać ten problem, Usuń istniejącą grupę, jeśli nie jest już potrzebna lub Utwórz witrynę z innym przypisanym aliasem.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="5d0c5-110">Istnieją różne sposoby tworzenia i używania nowoczesnych grup z programem SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="5d0c5-111">Istniejące witryny można połączyć z grupą 365 pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="5d0c5-112">Aby uzyskać więcej informacji, zobacz [łączenie grupy 365 pakietu Office za pomocą ineterface użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="5d0c5-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="5d0c5-113">Aby utworzyć witrynę grupy 365 pakietu Office, należy utworzyć witrynę zespołu.</span><span class="sxs-lookup"><span data-stu-id="5d0c5-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="5d0c5-114">Aby uzyskać więcej informacji, zobacz [Tworzenie witryny zespołu w programie SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="5d0c5-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>


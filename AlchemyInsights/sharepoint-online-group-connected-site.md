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
ms.openlocfilehash: 049ef5acd80d64e00315ba07f274567e6a251904
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642154"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="ab312-102">Problemy podczas tworzenia witryny połączonej z grupą w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="ab312-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="ab312-103">Niektóre typowe problemy napotkane podczas tworzenia lub ponownego tworzenia witryny połączonej z grupą.</span><span class="sxs-lookup"><span data-stu-id="ab312-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="ab312-104">Jeśli grupa i jej połączona witryna zostały usunięte i chcesz utworzyć inną witrynę o tym samym adresie URL, musisz trwale usunąć poprzednią witrynę.</span><span class="sxs-lookup"><span data-stu-id="ab312-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="ab312-105">Pobierz [powłokę zarządzania SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="ab312-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="ab312-106">Aby uzyskać więcej informacji na temat rozpoczynania pracy z programem Powershell, zobacz [Wprowadzenie do powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="ab312-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="ab312-107">Usuń witrynę z usuniętych witryn za pomocą polecenia cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="ab312-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="ab312-108">Program Powershell jest wymagany do trwałego usuwania witryn grupowych.</span><span class="sxs-lookup"><span data-stu-id="ab312-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="ab312-109">Jeśli tworzysz witrynę połączoną z grupą i otrzymujesz ostrzeżenie: **Inna grupa o tym samym aliasie już istnieje,** sprawdź istniejące grupy z Centrum [administracyjnego usługi Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="ab312-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="ab312-110">Aby rozwiązać ten problem, usuń istniejącą grupę, jeśli nie jest już potrzebna, lub utwórz witrynę z przypisanym innym aliasem.</span><span class="sxs-lookup"><span data-stu-id="ab312-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="ab312-111">Istnieją różne sposoby tworzenia i używania nowoczesnych grup w programie SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ab312-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="ab312-112">Istniejące witryny można połączyć z grupą usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="ab312-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="ab312-113">Aby uzyskać więcej informacji, zobacz [Łączenie grupy usługi Office 365 przy użyciu interfejsu użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="ab312-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="ab312-114">Aby utworzyć witrynę połączoną z grupą usługi Office 365, musisz utworzyć [witrynę zespołu](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="ab312-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>

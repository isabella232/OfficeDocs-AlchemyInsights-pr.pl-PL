---
title: Dodawanie grupy do witryny programu SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771218"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="9ac23-102">Problemy podczas tworzenia witryny połączonej z grupą w programie SharePoint</span><span class="sxs-lookup"><span data-stu-id="9ac23-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="9ac23-103">Napotkano niektóre typowe problemy podczas tworzenia lub ponownego tworzenia witryny połączonej z grupą.</span><span class="sxs-lookup"><span data-stu-id="9ac23-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="9ac23-104">Jeśli usunięto grupę i jej połączoną witrynę i chcesz utworzyć inną witrynę o tym samym adresie URL, musisz trwale usunąć poprzednią witrynę.</span><span class="sxs-lookup"><span data-stu-id="9ac23-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="9ac23-105">Pobierz [powłokę zarządzania usługi spo](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="9ac23-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="9ac23-106">Aby uzyskać więcej informacji na temat rozpoczynania pracy z programem PowerShell, zobacz [wprowadzenie do powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="9ac23-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="9ac23-107">Usuń witrynę z witryn usuniętych za pomocą polecenia cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9ac23-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="9ac23-108">Do trwałego usunięcia witryn grupy jest wymagany program PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9ac23-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="9ac23-109">Jeśli tworzysz witrynę połączoną z grupą i otrzymujesz Ostrzeżenie: **inna grupa o tym samym aliasie już istnieje**, Sprawdź istniejące grupy w [centrum administracyjnym usługi Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="9ac23-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="9ac23-110">Aby rozwiązać ten problem, Usuń istniejącą grupę, jeśli nie jest już potrzebna, lub Utwórz witrynę z przypisanym innym aliasem.</span><span class="sxs-lookup"><span data-stu-id="9ac23-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="9ac23-111">Istnieją różne sposoby tworzenia i używania nowoczesnych grup w programie SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9ac23-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="9ac23-112">Istniejące witryny można połączyć z grupą programu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ac23-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="9ac23-113">Aby uzyskać więcej informacji, zobacz [łączenie grupy programu Microsoft 365 za pomocą interfejsu użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="9ac23-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="9ac23-114">Aby utworzyć witrynę połączoną z grupą programu Microsoft 365, należy utworzyć [witrynę zespołu](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="9ac23-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>

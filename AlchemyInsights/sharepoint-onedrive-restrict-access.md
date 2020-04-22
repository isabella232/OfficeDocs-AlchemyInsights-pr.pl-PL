---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692775"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="751d5-102">Ograniczanie dostępu w programie SharePoint lub OneDrive</span><span class="sxs-lookup"><span data-stu-id="751d5-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="751d5-103">Istnieje wiele sposobów ograniczania dostępu do usług usługi SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="751d5-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="751d5-104">Te różne metody ograniczeń dostępu są opisane poniżej.</span><span class="sxs-lookup"><span data-stu-id="751d5-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="751d5-105">**Ograniczenie uprawnień**</span><span class="sxs-lookup"><span data-stu-id="751d5-105">**Permission Restriction**</span></span>

<span data-ttu-id="751d5-106">W usłudze SharePoint Online i usłudze OneDrive dla Firm ograniczamy dostęp do elementów, takich jak witryny, pliki i foldery, przyznając dostęp tylko tym grupom/osobom, które powinny mieć dostęp.</span><span class="sxs-lookup"><span data-stu-id="751d5-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="751d5-107">Dostosowywanie uprawnień do listy lub biblioteki programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="751d5-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="751d5-108">Dostosowywanie uprawnień witryny programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="751d5-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="751d5-109">Zmienianie uprawnień w podfolderze</span><span class="sxs-lookup"><span data-stu-id="751d5-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="751d5-110">Sterowanie dostępem z poziomu urządzeń niezarządzanych</span><span class="sxs-lookup"><span data-stu-id="751d5-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="751d5-111">Jako administrator programu SharePoint lub administrator globalny możesz blokować lub ograniczać dostęp do zawartości programu SharePoint i OneDrive z urządzeń niezarządzanych (tych, które nie są przyłączone do usługi AD hybrydowej lub są zgodne w usłudze Intune).</span><span class="sxs-lookup"><span data-stu-id="751d5-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="751d5-112">**Ograniczenie lokalizacji sieciowej**</span><span class="sxs-lookup"><span data-stu-id="751d5-112">**Network Location Restriction**</span></span>

<span data-ttu-id="751d5-113">Jako administrator IT możesz kontrolować dostęp do zasobów programu SharePoint i OneDrive na podstawie zaufanych lokalizacji sieciowych.</span><span class="sxs-lookup"><span data-stu-id="751d5-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="751d5-114">Jest to również znane jako zasady oparte na lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="751d5-114">This is also known as location-based policy.</span></span> <span data-ttu-id="751d5-115">Aby uzyskać więcej informacji, zobacz [Kontrolowanie dostępu do danych usługi SharePoint Online i OneDrive na podstawie lokalizacji sieciowej](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="751d5-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="751d5-116">**Ograniczenie blokady witryny**</span><span class="sxs-lookup"><span data-stu-id="751d5-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="751d5-117">W usłudze SharePoint Online masz możliwość zablokowania zbioru witryn, więc nikt nie ma do niego dostępu.</span><span class="sxs-lookup"><span data-stu-id="751d5-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="751d5-118">Jest to ustawiane za pośrednictwem programu PowerShell i [powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) przy użyciu właściwości [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="751d5-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="751d5-119">**Ograniczanie użytkownikom tworzenia witryn lub podwitryn**</span><span class="sxs-lookup"><span data-stu-id="751d5-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="751d5-120">Jako administrator programu SharePoint lub administrator globalny możesz pozwolić użytkownikom tworzyć własne witryny programu SharePoint i administrować nimi, określać, jakiego rodzaju witryny mogą tworzyć, oraz określać lokalizację witryn.</span><span class="sxs-lookup"><span data-stu-id="751d5-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="751d5-121">Aby uzyskać więcej informacji, zobacz [Zarządzanie tworzeniem witryny w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="751d5-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>


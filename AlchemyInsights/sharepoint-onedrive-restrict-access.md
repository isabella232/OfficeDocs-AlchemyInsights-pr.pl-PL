---
title: Ograniczanie dostępu w programie SharePoint lub usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700465"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="7e343-102">Ograniczanie dostępu w programie SharePoint lub usłudze OneDrive</span><span class="sxs-lookup"><span data-stu-id="7e343-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="7e343-103">Istnieje wiele sposobów ograniczania dostępu do usług SharePoint Online i OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7e343-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="7e343-104">Te różnorodne metody ograniczeń dostępu przedstawiono poniżej.</span><span class="sxs-lookup"><span data-stu-id="7e343-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="7e343-105">**Ograniczenia uprawnień**</span><span class="sxs-lookup"><span data-stu-id="7e343-105">**Permission Restriction**</span></span>

<span data-ttu-id="7e343-106">W usłudze SharePoint Online i usłudze OneDrive dla firm ograniczenie dostępu do elementów, takich jak witryny, pliki i foldery, jest udzielane tylko użytkownikom, którzy powinni mieć dostęp.</span><span class="sxs-lookup"><span data-stu-id="7e343-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="7e343-107">Dostosowywanie uprawnień do listy lub biblioteki programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="7e343-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="7e343-108">Dostosowywanie uprawnień do witryny programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="7e343-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="7e343-109">Zmienianie uprawnień w podfolderze</span><span class="sxs-lookup"><span data-stu-id="7e343-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="7e343-110">Sterowanie dostępem z poziomu urządzeń niezarządzanych</span><span class="sxs-lookup"><span data-stu-id="7e343-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="7e343-111">Jako administrator programu SharePoint lub administratora globalnego możesz zablokować lub ograniczyć dostęp do zawartości programu SharePoint i usługi OneDrive z urządzeń niezarządzanych (tych, które nie są dołączone lub są zgodne z usługą Intune).</span><span class="sxs-lookup"><span data-stu-id="7e343-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="7e343-112">**Ograniczenie lokalizacji sieciowej**</span><span class="sxs-lookup"><span data-stu-id="7e343-112">**Network Location Restriction**</span></span>

<span data-ttu-id="7e343-113">Jako administrator IT możesz kontrolować dostęp do zasobów programu SharePoint i usługi OneDrive na podstawie zdefiniowanych lokalizacji sieciowych, którym ufasz.</span><span class="sxs-lookup"><span data-stu-id="7e343-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="7e343-114">Jest to również nazywane zasadami opartymi na lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="7e343-114">This is also known as location-based policy.</span></span> <span data-ttu-id="7e343-115">Aby uzyskać więcej informacji, zobacz [kontrolowanie dostępu do usługi SharePoint Online i danych usługi OneDrive na podstawie lokalizacji sieciowej](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) .</span><span class="sxs-lookup"><span data-stu-id="7e343-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="7e343-116">**Ograniczenie blokady witryny**</span><span class="sxs-lookup"><span data-stu-id="7e343-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="7e343-117">W usłudze SharePoint Online możesz zablokować zbiór witryn, więc nikt nie ma dostępu.</span><span class="sxs-lookup"><span data-stu-id="7e343-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="7e343-118">Jest ona ustawiana za pośrednictwem programu PowerShell i [powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) przy użyciu właściwości [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="7e343-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="7e343-119">**Ograniczanie użytkowników do tworzenia witryn i podwitryn**</span><span class="sxs-lookup"><span data-stu-id="7e343-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="7e343-120">Jako administrator programu SharePoint lub Administrator globalny możesz umożliwić użytkownikom tworzenie i administrowanie swoimi witrynami programu SharePoint, Określanie rodzaju witryn, które mogą tworzyć, oraz Określanie lokalizacji witryn.</span><span class="sxs-lookup"><span data-stu-id="7e343-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="7e343-121">Aby uzyskać więcej informacji, zobacz [Zarządzanie tworzeniem witryn w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="7e343-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>


---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750674"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="83a77-102">Ograniczanie dostępu w programie SharePoint lub OneDrive</span><span class="sxs-lookup"><span data-stu-id="83a77-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="83a77-103">Istnieje wiele sposobów ograniczania dostępu do usług SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="83a77-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="83a77-104">Te różne metody ograniczania dostępu są opisane poniżej.</span><span class="sxs-lookup"><span data-stu-id="83a77-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="83a77-105">**Ograniczenie uprawnień**</span><span class="sxs-lookup"><span data-stu-id="83a77-105">**Permission Restriction**</span></span>

<span data-ttu-id="83a77-106">W programie SharePoint Online i OneDrive dla firm możemy ograniczyć dostęp do elementów, takich jak witryny, pliki i foldery, udzielając tylko dostępu do tych grup/osób, które powinny mieć dostęp.</span><span class="sxs-lookup"><span data-stu-id="83a77-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="83a77-107">Dostosowywanie uprawnień do listy lub biblioteki programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="83a77-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="83a77-108">Dostosowywanie uprawnień witryny programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="83a77-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="83a77-109">Zmienianie uprawnień do podfolderu</span><span class="sxs-lookup"><span data-stu-id="83a77-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="83a77-110">Sterowanie dostępem z poziomu urządzeń niezarządzanych</span><span class="sxs-lookup"><span data-stu-id="83a77-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="83a77-111">Jako administrator programu SharePoint lub globalnego w pakiecie Office 365, można zablokować lub ograniczyć dostęp do zawartości programu SharePoint i OneDrive z niezarządzanych urządzeń (te nie hybrydowy AD przyłączony lub zgodny w usłudze Intune).</span><span class="sxs-lookup"><span data-stu-id="83a77-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="83a77-112">**Ograniczenie lokalizacji sieciowej**</span><span class="sxs-lookup"><span data-stu-id="83a77-112">**Network Location Restriction**</span></span>

<span data-ttu-id="83a77-113">Administrator IT może kontrolować dostęp do zasobów programu SharePoint i usługi OneDrive na podstawie zdefiniowanych zaufanych lokalizacji sieciowych.</span><span class="sxs-lookup"><span data-stu-id="83a77-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="83a77-114">Jest to również nazywane zasadami opartymi na lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="83a77-114">This is also known as location-based policy.</span></span> <span data-ttu-id="83a77-115">Aby uzyskać więcej informacji, zobacz [Kontrola dostępu do usługi SharePoint Online i OneDrive danych w oparciu o lokalizację sieciową](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="83a77-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="83a77-116">**Ograniczenie blokady witryny**</span><span class="sxs-lookup"><span data-stu-id="83a77-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="83a77-117">W programie SharePoint Online masz możliwość blokowania zbioru witryn, więc nikt nie ma dostępu.</span><span class="sxs-lookup"><span data-stu-id="83a77-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="83a77-118">Jest to ustawiane za pomocą programu PowerShell i [powłoki zarządzania programu SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) za pomocą właściwości [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="83a77-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="83a77-119">**Ograniczanie użytkownikom możliwości tworzenia witryn lub podwitryn**</span><span class="sxs-lookup"><span data-stu-id="83a77-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="83a77-120">Jako administrator programu SharePoint lub Office 365 globalnego administratora, możesz pozwolić użytkownikom na tworzenie i administrowanie własnymi witrynami programu SharePoint, określić, jakiego rodzaju witryn mogą tworzyć i określić lokalizację witryn.</span><span class="sxs-lookup"><span data-stu-id="83a77-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="83a77-121">Aby uzyskać więcej informacji, zobacz [Zarządzanie tworzeniem witryny w programie SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="83a77-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>


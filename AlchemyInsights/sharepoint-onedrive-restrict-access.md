---
title: Ograniczanie dostępu w programie SharePoint lub OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223722"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="65821-102">Ograniczanie dostępu w programie SharePoint lub OneDrive</span><span class="sxs-lookup"><span data-stu-id="65821-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="65821-103">Istnieje wiele sposobów, aby ograniczyć dostęp do usług SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="65821-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="65821-104">Te różne metody ograniczania dostępu są przedstawione poniżej.</span><span class="sxs-lookup"><span data-stu-id="65821-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="65821-105">**Ograniczenie uprawnień**</span><span class="sxs-lookup"><span data-stu-id="65821-105">**Permission Restriction**</span></span>

<span data-ttu-id="65821-106">W SharePoint Online i OneDrive dla firmy możemy ograniczyć dostęp do elementów, takich jak witryny, pliki i foldery tylko udzielenie dostępu do tych grup/użytkowników, którzy powinni mieć dostęp.</span><span class="sxs-lookup"><span data-stu-id="65821-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="65821-107">Dostosowywanie uprawnień dla listy programu SharePoint lub biblioteki</span><span class="sxs-lookup"><span data-stu-id="65821-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="65821-108">Dostosowywanie uprawnień witryny programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="65821-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="65821-109">Należy zmienić uprawnienia do podfolderu</span><span class="sxs-lookup"><span data-stu-id="65821-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="65821-110">Sterowanie dostępem z poziomu urządzeń niezarządzanych</span><span class="sxs-lookup"><span data-stu-id="65821-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="65821-111">Jako programu SharePoint lub administratora globalnego w usłudze Office 365, możesz zablokować lub ograniczyć dostęp do zawartości programu SharePoint i OneDrive z niezarządzanych urządzeń (tych mieszańców AD sprzężone lub zgodny w usłudze Intune).</span><span class="sxs-lookup"><span data-stu-id="65821-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="65821-112">**Ograniczenia lokalizacji w sieci**</span><span class="sxs-lookup"><span data-stu-id="65821-112">**Network Location Restriction**</span></span>

<span data-ttu-id="65821-113">Jako administrator można kontrolować dostęp do zasobów programu SharePoint i OneDrive w oparciu o zaufanych lokalizacji sieci.</span><span class="sxs-lookup"><span data-stu-id="65821-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="65821-114">To jest również znany jako zasad opartych na lokalizacji.</span><span class="sxs-lookup"><span data-stu-id="65821-114">This is also known as location-based policy.</span></span> <span data-ttu-id="65821-115">Aby uzyskać więcej informacji zobacz [Kontrola dostępu do programu SharePoint w trybie Online i OneDrive dane oparte na lokalizacji sieciowej](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="65821-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="65821-116">**Ograniczenia blokowanie witryny**</span><span class="sxs-lookup"><span data-stu-id="65821-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="65821-117">W ramach programu SharePoint w trybie Online mają zdolność do blokowania zbioru witryn, dlatego nikt nie ma dostępu.</span><span class="sxs-lookup"><span data-stu-id="65821-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="65821-118">To jest ustawiany za pomocą środowiska PowerShell i [Online powłoki zarządzania programu SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) przy użyciu właściwości - LockState [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="65821-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="65821-119">**Zabronić użytkownikom tworzenie witryn i podwitryn**</span><span class="sxs-lookup"><span data-stu-id="65821-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="65821-120">Jako administrator programu SharePoint lub globalnego administratora usługi Office 365, można pozwolić użytkownikom tworzyć i administrować własnych witryn programu SharePoint, określić, jakiego rodzaju witryn mogą utworzyć, a następnie określ lokalizację witryny.</span><span class="sxs-lookup"><span data-stu-id="65821-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="65821-121">Aby uzyskać więcej informacji zobacz [Tworzenie witryny Zarządzanie w dokumentacji Online programu SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="65821-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>


---
title: Wdrażanie dodatków dla aplikacji Aplikacje Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233544"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="82463-102">Wdrażanie dodatków dla aplikacji Aplikacje Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="82463-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="82463-103">Scentralizowane wdrażanie to zalecany sposób wdrażania dodatków Office użytkowników i grup w organizacji.</span><span class="sxs-lookup"><span data-stu-id="82463-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="82463-104">Aby wdrożyć dodatki, wykonaj poniższe czynności:</span><span class="sxs-lookup"><span data-stu-id="82463-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="82463-105">**Uwaga:** Aby zainstalować dodatki dla użytkowników Office użytkowników, zobacz Wyświetlanie i instalowanie dodatków oraz zarządzanie nimi w [Office programów.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="82463-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="82463-106">Upewnij się też, że jest włączone indywidualne Office dodatków ze Sklepu.</span><span class="sxs-lookup"><span data-stu-id="82463-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="82463-107">Aby uzyskać szczegółowe informacje, zobacz Uniemożliwianie pobierania dodatków przez wyłączenie [Sklepu Office wszystkich](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)klientów (z wyjątkiem Outlook).</span><span class="sxs-lookup"><span data-stu-id="82463-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="82463-108">Upewnij się, że Twoje środowisko spełnia wymagania dotyczące wdrażania dodatków przy użyciu funkcji scentralizowanego wdrażania.</span><span class="sxs-lookup"><span data-stu-id="82463-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="82463-109">Aby uzyskać szczegółowe informacje, zobacz [Wymagania.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="82463-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="82463-110">Przejdź do **Ustawienia**  >  **zintegrowane aplikacje** Uzyskaj aplikacje w centrum administracyjnym usługi Microsoft 365, aby wdrożyć  >   dodatki.</span><span class="sxs-lookup"><span data-stu-id="82463-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="82463-111">Uwagi:</span><span class="sxs-lookup"><span data-stu-id="82463-111">Notes:</span></span> 

- <span data-ttu-id="82463-112">Zintegrowane aplikacje wymagają, aby administrator ma uprawnienia administratora globalnego Exchange administratora.</span><span class="sxs-lookup"><span data-stu-id="82463-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="82463-113">W przypadku wdrażania dodatków u wielu użytkowników zalecamy przypisywanie ich przy użyciu grup, a nie pojedynczych użytkowników.</span><span class="sxs-lookup"><span data-stu-id="82463-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="82463-114">Aby uzyskać szczegółowe informacje, zobacz Zagadnienia dotyczące przypisywania dodatku [do użytkowników i grup.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="82463-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="82463-115">Scentralizowane wdrażanie nie obsługuje użytkowników w zagnieżdżonych grupach, które mają grupy nadrzędne.</span><span class="sxs-lookup"><span data-stu-id="82463-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="82463-116">Aby uzyskać szczegółowe informacje, [zobacz Przydziały użytkowników i grup.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="82463-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="82463-117">Upewnij się, że usługa zarządzania Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') jest włączona dla użytkowników w celu zalogowania się.</span><span class="sxs-lookup"><span data-stu-id="82463-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="82463-118">Aby uzyskać szczegółowe informacje, [zobacz Konfigurowanie właściwości aplikacji.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="82463-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="82463-119">Jeśli podczas wdrażania dodatków za pomocą zintegrowanych aplikacji wystąpią problemy, spróbuj wdrożyć je przy użyciu [dodatków.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="82463-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="82463-120">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="82463-120">For more information, see:</span></span>

<span data-ttu-id="82463-121">[Wdrażanie dodatków w centrum administracyjnym](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Zarządzanie dodatki w centrum administracyjnym](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Zarządzanie dodatkimi przy użyciu poleceń cmdlet](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) programu PowerShell dla funkcji Scentralizowane wdrażanie 
 Publikowanie Office przy użyciu [funkcji scentralizowanego wdrażania za](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) pośrednictwem Microsoft 365 administracyjnego 
 [Rozwiązywanie problemów: Użytkownik nie widzi dodatków](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Rozwiązywanie problemów użytkowników z Office dodatków](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="82463-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>
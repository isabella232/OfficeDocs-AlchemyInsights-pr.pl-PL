---
title: Problemy dotyczące właściciela rejestracji aplikacji
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404780"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="bc962-102">Problemy dotyczące właściciela rejestracji aplikacji</span><span class="sxs-lookup"><span data-stu-id="bc962-102">App Registration Owner issues</span></span>

<span data-ttu-id="bc962-103">Poniżej przedstawiono dostępne metody dodawania podmiotów głównych jako właścicieli rejestracji aplikacji:</span><span class="sxs-lookup"><span data-stu-id="bc962-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="bc962-104">Moduł PowerShell usługi Azure AD —</span><span class="sxs-lookup"><span data-stu-id="bc962-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="bc962-105">Informacje: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="bc962-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="bc962-106">Korzystanie z funkcji Azure CLI — `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="bc962-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="bc962-107">Informacje: [właściciel aplikacji az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="bc962-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="bc962-108">Używanie funkcji MS Graph —</span><span class="sxs-lookup"><span data-stu-id="bc962-108">Using MS Graph -</span></span>

    <span data-ttu-id="bc962-109">Informacje: [Dodawanie właściciela — Microsoft Graph w wersji 1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="bc962-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="bc962-110">Korzystanie z portalu usługi Azure AD — przejdź do portal.azure.com [>](https://portal.azure.com/) usługi Azure Active Directory > rejestracja aplikacji > Wybierz aplikację > Właściciele > Dodaj właścicieli</span><span class="sxs-lookup"><span data-stu-id="bc962-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="bc962-111">**Nie możesz wyświetlić aplikacji na tablicy rejestracji aplikacji, nawet jeśli jesteś właścicielem tej aplikacji?**</span><span class="sxs-lookup"><span data-stu-id="bc962-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="bc962-112">Właściciel aplikacji nie jest rolą administracyjną.</span><span class="sxs-lookup"><span data-stu-id="bc962-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="bc962-113">Jeśli ustawienie Ogranicz dostęp do portalu administracyjnego [usługi Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) jest włączone, tylko administrator będzie mógł wyświetlać aplikacje w portalu rejestracji aplikacji.</span><span class="sxs-lookup"><span data-stu-id="bc962-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="bc962-114">Aby właściciel mógł wyświetlać aplikacje, wyłącz to ustawienie (Ustaw to na wartość NIE) lub przypisz rolę administratora tylko do konkretnej aplikacji.</span><span class="sxs-lookup"><span data-stu-id="bc962-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="bc962-115">Jednak w tym celu należy wymagać licencji Azure AD Premium P2 i włączyć [zarządzanie tożsamością privileged.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="bc962-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>

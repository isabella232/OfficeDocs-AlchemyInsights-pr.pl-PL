---
title: Zasady grupy
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256783"
---
# <a name="group-policy"></a><span data-ttu-id="a8319-102">Zasady grupy</span><span class="sxs-lookup"><span data-stu-id="a8319-102">Group policy</span></span>

<span data-ttu-id="a8319-103">Ustawieniami obiektów użytkowników i komputerów w usłudze Azure Usługi domenowe w usłudze Active Directory (Azure AD DS) często zarządza się przy użyciu obiektów zasady grupy (GPO).</span><span class="sxs-lookup"><span data-stu-id="a8319-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="a8319-104">Usługa Azure AD DS zawiera wbudowane urządzenia GPO dla kontenerów Użytkowników usługi AADDC i komputerów usługi AADDC.</span><span class="sxs-lookup"><span data-stu-id="a8319-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="a8319-105">Te wbudowane zasady grupy można dostosowywać w celu skonfigurowania zasad grupy zgodnie z potrzebami środowiska.</span><span class="sxs-lookup"><span data-stu-id="a8319-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="a8319-106">Członkowie grupy administratorów centrum administracyjnego usługi Azure AD mają uprawnienia do administrowania zasadami grupy w domenie usługi Azure AD DS, a także mogą tworzyć niestandardowe grupy gpos i jednostki organizacyjne.</span><span class="sxs-lookup"><span data-stu-id="a8319-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="a8319-107">Aby uzyskać więcej informacji na temat zasad grupy i ich działania, zobacz [zasady grupy omówienie.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="a8319-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="a8319-108">W środowisku hybrydowym zasady grupy skonfigurowane w lokalnym środowisku AD DS nie są synchronizowane z usługą Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="a8319-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="a8319-109">Aby zdefiniować ustawienia konfiguracji dla użytkowników lub komputerów w usłudze Azure AD DS, edytuj jedno z domyślnych zasad grupy lub utwórz niestandardowy obiektów zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="a8319-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="a8319-110">W tym [artykule zasady grupy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) przedstawiono sposób instalowania narzędzi do zarządzania zasady grupy, edytowania wbudowanych zasad grupy oraz tworzenia niestandardowych zasad grupy.</span><span class="sxs-lookup"><span data-stu-id="a8319-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>




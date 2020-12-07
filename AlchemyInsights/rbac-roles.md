---
title: 'Role RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583948"
---
# <a name="rbac-rules"></a><span data-ttu-id="61306-102">Reguły RBAC</span><span class="sxs-lookup"><span data-stu-id="61306-102">RBAC rules</span></span>

<span data-ttu-id="61306-103">Jeśli zostanie wyświetlony błąd uprawnień:</span><span class="sxs-lookup"><span data-stu-id="61306-103">If you get the permission error:</span></span> 

- <span data-ttu-id="61306-104">**Klient z identyfikatorem obiektu nie ma autoryzacji do wykonywania akcji w zakresie (kod: AuthorizationFailed)**: podczas próby utworzenia zasobu upewnij się, że zalogowano się przy użyciu użytkownika, któremu przypisano rolę z uprawnieniami do zapisu dla zasobu w wybranym zakresie.</span><span class="sxs-lookup"><span data-stu-id="61306-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="61306-105">Aby na przykład zarządzać maszynami wirtualnymi w grupie zasobów, należy mieć rolę [współautora maszyny wirtualnej](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) w grupie zasobów (lub zakresie nadrzędnym).</span><span class="sxs-lookup"><span data-stu-id="61306-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="61306-106">Aby uzyskać listę uprawnień poszczególnych ról wbudowanych, zobacz [wbudowane role dla zasobów platformy Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="61306-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="61306-107">**Nie masz uprawnień do tworzenia prośby** o szczegółowe dane: podczas próby utworzenia lub zaktualizowania biletu pomocy technicznej upewnij się, że zalogowano się do użytkownika, któremu przypisano rolę z uprawnieniem Microsoft. Support/supportTickets/Write, na przykład [współautorze prośby o pomoc](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="61306-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="61306-108">**Nie można utworzyć więcej przypisań ról (kod: RoleAssignmentLimitExceeded)**: podczas próby przypisania roli spróbuj zmniejszyć liczbę przypisań ról, przypisując role do grup.</span><span class="sxs-lookup"><span data-stu-id="61306-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="61306-109">Platforma Azure obsługuje do **2000** przydziały ról na abonament.</span><span class="sxs-lookup"><span data-stu-id="61306-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="61306-110">Aby uzyskać więcej szczegółowych informacji na temat ról usługi Azure RBAC, zobacz [role usługi Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="61306-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

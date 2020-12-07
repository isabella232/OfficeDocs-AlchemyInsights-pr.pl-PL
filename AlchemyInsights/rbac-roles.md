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
# <a name="rbac-rules"></a>Reguły RBAC

Jeśli zostanie wyświetlony błąd uprawnień: 

- **Klient z identyfikatorem obiektu nie ma autoryzacji do wykonywania akcji w zakresie (kod: AuthorizationFailed)**: podczas próby utworzenia zasobu upewnij się, że zalogowano się przy użyciu użytkownika, któremu przypisano rolę z uprawnieniami do zapisu dla zasobu w wybranym zakresie. Aby na przykład zarządzać maszynami wirtualnymi w grupie zasobów, należy mieć rolę [współautora maszyny wirtualnej](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) w grupie zasobów (lub zakresie nadrzędnym). Aby uzyskać listę uprawnień poszczególnych ról wbudowanych, zobacz [wbudowane role dla zasobów platformy Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Nie masz uprawnień do tworzenia prośby** o szczegółowe dane: podczas próby utworzenia lub zaktualizowania biletu pomocy technicznej upewnij się, że zalogowano się do użytkownika, któremu przypisano rolę z uprawnieniem Microsoft. Support/supportTickets/Write, na przykład [współautorze prośby o pomoc](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Nie można utworzyć więcej przypisań ról (kod: RoleAssignmentLimitExceeded)**: podczas próby przypisania roli spróbuj zmniejszyć liczbę przypisań ról, przypisując role do grup. Platforma Azure obsługuje do **2000** przydziały ról na abonament.

Aby uzyskać więcej szczegółowych informacji na temat ról usługi Azure RBAC, zobacz [role usługi Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923141"
---
# <a name="rbac-rules"></a>Reguły RBAC

Jeśli zostanie komunikat o błędzie uprawnień: 

- Klient z identyfikatorem obiektu nie ma autoryzacji do wykonywania akcji w zakresie **(kod: AutoryzacjaFailed):** podczas próby utworzenia zasobu sprawdź, czy użytkownik, do którym przypisano rolę zapisu w wybranym zakresie, jest obecnie zalogowany do Ciebie. Aby na przykład zarządzać maszynami wirtualnymi w [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) grupie zasobów, w grupie zasobów powinna być pełnić rolę współautora maszyn wirtualnych w grupie zasobów (lub zakresie nadrzędnym). Aby uzyskać listę uprawnień dla poszczególnych wbudowanych ról, zobacz Role wbudowane dla [zasobów platformy Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Nie masz uprawnień do utworzenia wniosku o pomoc **techniczną:** podczas próby utworzenia lub zaktualizowania biletu do pomocy technicznej sprawdź, czy aktualnie jesteś zalogowany u użytkownika z przypisaną rolą, która ma uprawnienie Microsoft.Support/supportTickets/write, takie jak Współautor wniosku o pomoc [techniczną.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Nie można tworzyć więcej przypisań ról **(kod: RolaAssignmentLimitExceeded),** gdy próbujesz przypisać rolę, spróbuj zmniejszyć liczbę przypisań ról, przypisując role do grup. Platforma Azure obsługuje **maksymalnie 2000** przypisań ról na subskrypcję.

Aby uzyskać więcej szczegółowych informacji o rolach usługi Azure RBAC, zobacz [Role usługi Azure RBAC.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

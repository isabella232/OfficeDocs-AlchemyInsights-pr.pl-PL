---
title: Problemy z korzystaniem z konsoli administracyjnej usługi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555388"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemy z korzystaniem z konsoli administracyjnej usługi Intune

**"Odmowa dostępu" podczas nawigacji po portalu administracyjnym usługi Intune.**

- Jeśli jesteś członkiem roli niestandardowej usługi Intune, upewnij się, że do Twojego konta jest przypisana licencja usługi Intune lub Enterprise Mobility Suite (EMS).
- Jeśli do zarządzania urządzeniami używasz programu Menedżer konfiguracji, sprawdź, czy nie należysz do kolekcji użytkowników usługi Intune dla programu MDM programu Configuration Manager.
- Sprawdź, czy w bloku role usługi Intune przypisano odpowiednie uprawnienia kontroli administracji opartej na rolach (RBAC).
- Sprawdź, czy używana grupa nie jest listą dystrybucyjną. Usługa Intune w portalu Azure obsługuje tylko konta użytkowników należących do grup zabezpieczeń usługi Azure Active Directory. Przejrzyj swoje grupy w witrynie Azure portal > grupy **usługi Intune**  >  **Groups**lub w witrynie Azure portal > usługi Azure **Active Directory**.

**Użytkownik ma zbyt wiele uprawnień dla przypisanej roli usługi Intune**

Należy zaradzić użytkownikowi, aby przejść do ról **usługi**  >  **Intune Usługi Intune**  >  **Moje uprawnienia**  >  **Eksportuj** do przeglądu przyznanych uprawnień.

**Dodałem grupę zakresu do roli, ale użytkownicy w tej roli nadal widzą innych użytkowników lub urządzenia.**

Grupy zakresów nie odfiltrowują użytkowników ani urządzeń. Grupy zakresów:

- Ogranicz, do kogo użytkownicy mogą przypisywać zasady lub aplikacje.
- Zezwalaj tylko określonym użytkownikom na uruchamianie zadań zdalnych na urządzeniach.

Aby uzyskać więcej informacji na temat grup zakresów, zobacz [Kontrola dostępu oparta na rolach (RBAC) w usłudze Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Dodałem użytkownika do roli usługi Intune, ale nadal ma on pełny dostęp do konsoli administracyjnej usługi Intune.**

Przejdź do usługi Intune > **użytkownicy** w witrynie Azure portal i sprawdź, czy użytkownik nie jest przypisany do żadnej z następujących ról w witrynie Azure portal:

- Administrator globalny
- Administrator usługi usługi Intune
- Administrator usługi SharePoint

Aby uzyskać więcej informacji, zobacz [Kontrola dostępu oparta na rolach (RBAC) w usłudze Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemy z dostępem**

Aby uzyskać więcej informacji, zobacz [Nie można zalogować się do usługi Office 365, platformy Azure ani usługi Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).
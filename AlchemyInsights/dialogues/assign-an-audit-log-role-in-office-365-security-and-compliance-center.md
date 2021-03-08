---
title: Przypisywanie roli dziennika inspekcji w Centrum zgodności & zabezpieczeń usługi Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526525"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="6aed1-102">Przypisywanie roli dziennika inspekcji w Centrum zgodności & zabezpieczeń usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="6aed1-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="6aed1-103">Aby przeszukiwać dziennik inspekcji usługi Office 365,  administrator musi mieć przypisaną rolę Dzienniki inspekcji tylko do wyświetlania lub Dzienniki inspekcji w usłudze Exchange Online. </span><span class="sxs-lookup"><span data-stu-id="6aed1-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="6aed1-104">Te role są domyślnie przypisane do grup ról Zarządzanie zgodnością i Zarządzanie organizacją.</span><span class="sxs-lookup"><span data-stu-id="6aed1-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="6aed1-105">Administratorzy globalni w usłudze Office 365 i usłudze Microsoft 365 są automatycznie dodawana jako członkowie grupy ról Zarządzanie organizacją.</span><span class="sxs-lookup"><span data-stu-id="6aed1-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="6aed1-106">Aby umożliwić użytkownikowi wyszukiwanie z minimalnym poziomem uprawnień, utwórz niestandardową grupę  ról w udatku  Exchange Online, dodaj rolę Dzienniki inspekcji tylko do wyświetlania lub Dzienniki inspekcji, a następnie dodaj użytkownika jako członka nowej grupy ról.</span><span class="sxs-lookup"><span data-stu-id="6aed1-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="6aed1-107">Aby uzyskać więcej informacji, zobacz Zarządzanie grupami [ról w u](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) usługi Exchange Online i przeszukiwanie dziennika inspekcji w Centrum zabezpieczeń & [zgodności.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="6aed1-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749518"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Przypisywanie roli dziennika inspekcji w Centrum zgodności & zabezpieczeń usługi Office 365

Aby przeszukiwać dziennik inspekcji usługi Office 365,  administrator musi mieć przypisaną rolę Dzienniki inspekcji tylko do wyświetlania lub **Dzienniki** inspekcji w usłudze Exchange Online. Te role są domyślnie przypisane do grup ról Zarządzanie zgodnością i Zarządzanie organizacją. Administratorzy globalni usługi Office 365 i platformy Microsoft 365 są automatycznie dodawana jako członkowie grupy ról Zarządzanie organizacją.

Aby umożliwić użytkownikowi wyszukiwanie z minimalnym poziomem uprawnień, utwórz niestandardową grupę  ról w udatku  Exchange Online, dodaj rolę Dzienniki inspekcji tylko do wyświetlania lub Dzienniki inspekcji, a następnie dodaj użytkownika jako członka nowej grupy ról.

Aby uzyskać więcej informacji, zobacz [Zarządzanie grupami ról w u](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) usługi Exchange Online i Przeszukiwanie dziennika inspekcji w Centrum & [zabezpieczeń.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
---
title: Problem z grupami zabezpieczeń
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177627"
---
# <a name="issue-with-security-groups"></a>Problem z grupami zabezpieczeń

**Jeśli jest wyświetlany błąd sieci AADDS104**

Nieprawidłowe reguły grupy zabezpieczeń sieci są najczęstszą przyczyną błędów sieciowych w usłudze Azure Usługi domenowe w usłudze Active Directory (AD DS). Grupa zabezpieczeń sieci dla sieci wirtualnej musi zezwalać na dostęp do określonych portów i protokołów. Jeśli te porty są zablokowane, platforma Azure nie może monitorować ani aktualizować domeny zarządzanej. Ma to również wpływ na synchronizację między usługami Azure AD AD DS Azure. Upewnij się, że porty domyślne są otwarte, aby uniknąć przerw w działaniu usługi.

Aby zrozumieć i rozwiązać typowe alerty dotyczące problemów z konfiguracją grupy zabezpieczeń sieci, zobacz [Dodawanie i weryfikowanie grup zabezpieczeń.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)

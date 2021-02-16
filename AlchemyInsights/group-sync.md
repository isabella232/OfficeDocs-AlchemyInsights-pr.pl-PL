---
title: Synchronizacja grup
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
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256790"
---
# <a name="group-sync"></a>Synchronizacja grup

Ten artykuł zawiera wskazówki dotyczące synchronizacji grup.

1. Jeśli administrator globalny lub właściciel grupy nie może modyfikować właściwości grupy, dodawać członków ani przypisywać właścicieli w portalu Azure Portal, upewnij się, że źródłem uprawnień grupy jest usługa Azure Active Directory (Azure AD) dla administratora globalnego lub właściciela grupy w celu zmodyfikowania grupy.
2. Przed podjęciem próby usunięcia zsynchronizowanej grupy w [](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) usłudze Azure AD upewnij się, że usunięto wszystkie przypisane licencje, aby uniknąć błędów.

Aby dowiedzieć się, jak synchronizować użytkowników, grupy i kontakty, zobacz narzędzie [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)i postępuj zgodnie z synchronizować lokalną grupę z platformą Azure za pomocą programu Azure AD [Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) w celu synchronizowania grup w ramach programu AD Connect.

Aby rozwiązać typowe błędy podczas [synchronizacji,](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) postępuj zgodnie z tym przewodnikiem rozwiązywania problemów podczas synchronizacji.


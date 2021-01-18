---
title: Przypisywanie grup do roli usługi Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885393"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Przypisywanie grup do roli usługi Azure AD

Aby przypisać grupę usługi Azure AD za pomocą źródła uprawnień w usłudze Azure AD do roli usługi Azure AD, wykonaj następujące czynności:

1. Utwórz nową grupę — aby utworzyć nową grupę:

    a. Zaloguj się do centrum administracyjnego usługi Azure AD z uprawnieniami **administratora roli uprzywilejowanych** lub **administratora globalnego** .
    b. Wybierz pozycję **grupy usługi Azure Active Directory >, > wszystkie grupy > Nowa grupa**.
    c. Utwórz grupę.

2. Przypisz rolę do grupy podczas tworzenia grupy lub po utworzeniu grupy.

    a. Aby przypisać rolę do grupy w momencie tworzenia grupy, przełącz się na pozycję Przełącz **role usługi Azure AD do grupy** i Utwórz grupę.
    b. Aby przypisać rolę do grupy po jej utworzeniu, przejdź do karty **przypisane role** dla nowo utworzonej grupy i przypisz tę rolę grupie.  

**Zarządzanie członkostwem w grupie przypisanej do roli usługi Azure AD**

Aby zapobiec podnoszeniu uprawnień, domyślnie tylko Administratorzy ról uprzywilejowanych i Administratorzy globalni mogą modyfikować członkostwo grupy przypisanej do roli. Może jednak zdecydować o przypisaniu właściciela takiej grupy i delegować to zadanie.

Aby uzyskać więcej informacji na temat przypisywania grup w chmurze do ról usługi Azure AD, zobacz [Przypisywanie ról usługi AD do grupy chmury](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Aby uzyskać więcej informacji na temat rozwiązywania problemów z rolami przypisanymi do grup chmury, zobacz [Rozwiązywanie problemów z rolami przypisanymi do grup chmury](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).






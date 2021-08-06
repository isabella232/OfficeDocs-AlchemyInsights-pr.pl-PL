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
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036250"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Przypisywanie grup do roli usługi Azure AD

Aby przypisać grupę usługi Azure AD ze źródłem uprawnień w usłudze Azure AD do roli usługi Azure AD, wykonaj następujące czynności:

1. Tworzenie nowej grupy — aby utworzyć nową grupę:

    a. Zaloguj się do centrum administracyjnego usługi Azure AD z uprawnieniami **administratora roli lub** administratora **globalnego.**
    b. Wybierz **Azure Active Directory > Grupy > grupy > grupy > Nowa grupa.**
    c. Utwórz grupę.

2. Przypisz rolę do grupy podczas tworzenia grupy lub po jej utworzeniu.

    a. Aby podczas tworzenia grupy przypisać do grupy rolę, włącz przełącznik Ról usługi **Azure AD,** które można przypisać do grupy, i utwórz grupę.
    b. Aby przypisać rolę do grupy po jej utworzeniu, przejdź do karty Przypisane role dla nowo utworzonej grupy i przypisz tę rolę do grupy.   

**Zarządzanie członkostwem w grupie przypisanej do roli usługi Azure AD**

Aby uniemożliwić podwyższenie uprawnień, domyślnie tylko administratorzy ról z uprawnieniami i administratorzy globalni mogą modyfikować członkostwo w grupie przypisanej do roli. Mogą jednak zdecydować się na przypisanie właściciela do takiej grupy i delegowanie tego zadania.

Aby uzyskać więcej szczegółowych informacji na temat przypisywania grup w chmurze do ról usługi Azure AD, zobacz [Przypisywanie ról usługi AD do grupy w chmurze.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) Aby uzyskać więcej szczegółowych informacji na temat rozwiązywania problemów z rolami przypisanymi do grup w chmurze, zobacz Rozwiązywanie problemów z [rolami przypisanymi do grup w chmurze.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)






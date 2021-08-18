---
title: Jak dodawać administratorów i zarządzać nimi — zalecane czynności
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339042"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Jak dodawać administratorów i zarządzać nimi — zalecane czynności

Na podstawie opisu problemu znaleźliśmy rozwiązanie dla Ciebie. Większość klientów mogła rozwiązać swój problem samodzielnie po naszej dokumentacji.

**Edytowanie administratora subskrypcji lub współużytego administratora**

- Administrator konta może edytować obie role, natomiast administrator subskrypcji może zmieniać tylko administratorów współtworów w [Azure Portal.](https://ms.portal.azure.com/#home)
- [Dodawanie lub zmienianie administratorów subskrypcji platformy Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Aktualizowanie administratora subskrypcji lub Co-Administrator subskrypcji wewnętrznych (AIRS)**

Administrator usługi lub administrator współzawłasny mogą samodzielnie wykonać tę akcję, korzystając z następujących kroków:

1. Zaloguj się do portalu [Azure Portal](https://ms.portal.azure.com/#home) i kliknij pozycję Zarządzanie kosztami **+ Rozliczenia** w lewym okienku.
2. Kliknij pozycję w ramach subskrypcji. Spowoduje to otwarcie przeglądu subskrypcji.
3. Na bloku **Subskrypcji** kliknij pozycję **Właściwości**. 
4. Kliknij przycisk **Administrator usługi.**
5. Wprowadź adres e-mail użytkownika, którego chcesz ustawić jako administratora usługi, i kliknij przycisk **OK.**

**Add/Change/Remove Co-administrator**

1. Zaloguj się do [portalu Azure Portal](https://ms.portal.azure.com/#home) jako administrator usługi.
2. Otwórz [subskrypcje](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i wybierz subskrypcję. (Współ adminstratorów można przypisywać tylko w zakresie subskrypcji).
3. Przejdź do pozycji Administratorzy wersji klasycznej programu **Access (IAM),** aby otworzyć okienko Dodaj współ administratora (jeśli opcja Dodaj  >    >    >   współtworz administratora  jest wyłączona, oznacza to, że nie masz uprawnień).
4. Wybierz użytkownika, którego chcesz dodać, a następnie kliknij pozycję **Dodaj**.

**Dowiedz się więcej:**
- [Dodawanie administratora współtworzętego](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Usuwanie współwłasnych administratorów](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Zmienianie administratora usługi](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Wyświetlanie administratora konta](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Zarządzanie dostępem przy użyciu RBAC i Azure Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Dodawanie/usuwanie użytkowników przy Azure Active Directory (AD)**

Możesz dodawać nowych użytkowników lub usuwać istniejących użytkowników z organizacji usługi Azure Active Directory (Azure AD):

1. Aby dodać nowego użytkownika, zaloguj się w portalu [Azure Portal](https://ms.portal.azure.com/#home) jako administrator użytkownika w organizacji.
2. Wybierz **Azure Active Directory**, wybierz pozycję **Użytkownicy,** a następnie kliknij pozycję **Nowy użytkownik**.
3. Na **stronie Użytkownik** wypełnij wymagane informacje. Kliknij **przycisk Utwórz**. Użytkownik zostanie utworzony i dodany do Twojej dzierżawy usługi Azure AD.

**Dowiedz się więcej:**

- [Dodawanie nowego użytkownika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Usuwanie użytkownika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Dodawanie lub aktualizowanie informacji o profilu użytkownika przy użyciu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Polecane dokumenty**

- [Co to jest kontrola dostępu oparta na rolach?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Opis różnych ról na platformie Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Uprawnienia roli administratora w aplikacji Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Samouczek: udzielanie dostępu użytkownikowi za pomocą RBAC i Portalu Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Rozwiązywanie problemów z RBAC na platformie Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organizowanie zasobów za pomocą grup zarządzania azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Jak poprosić o kopię faktury za usługę Azure za pośrednictwem poczty e-mail](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Jak dodać, zaktualizować lub usunąć kartę kredytową lub debetową z platformy Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Zarządzaj subskrypcją (aktywuj ponownie/anuluj/przełącz)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)




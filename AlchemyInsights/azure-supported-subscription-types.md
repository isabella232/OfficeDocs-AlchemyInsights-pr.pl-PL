---
title: Obsługiwane typy subskrypcji
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820692"
---
# <a name="supported-subscription-types"></a>Obsługiwane typy subskrypcji

Aby kontynuować, przejrzyj obsługiwane typy subskrypcji.

[Obsługiwane typy subskrypcji](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Przenoszenie własności rozliczeń**

Zaloguj się do portalu Azure Portal jako [administrator konta](https://ms.portal.azure.com/) dla konta rozliczeniowego, które posiada subskrypcję, którą chcesz przenieść.

- Szukaj w pozycji **Zarządzanie kosztami + rozliczenia**. Wybierz pozycję **Subskrypcje** w okienku po lewej stronie. W zależności od dostępu może być konieczne wybranie zakresu rozliczeń, a następnie pozycji **Subskrypcje** lub **Subskrypcje platformy Azure**.
- Wybierz pozycję Przenieś własność rozliczeń dla subskrypcji, którą chcesz przenieść
- Wprowadź adres e-mail użytkownika, który jest administratorem rozliczeń konta, które będzie nowym właścicielem subskrypcji, a następnie wybierz pozycję **wyślij żądanie przeniesienia**
- Użytkownik otrzyma wiadomość e-mail z instrukcjami dotyczącymi rozpatrzenia żądania przeniesienia. Aby zatwierdzić żądanie przeniesienia, użytkownik wybiera link w wiadomości e-mail i postępuje zgodnie z instrukcjami.

Uwaga: jeśli przeniesiesz własność rozliczeń subskrypcji na konto użytkownika w innej dzierżawie usługi Azure Active Directory, wszystkie przypisania [kontroli dostępu na podstawie ról (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) do zarządzania zasobami w ramach subskrypcji zostaną trwale usunięte. Tylko nowy właściciel będzie mieć dostęp do zarządzania zasobami w ramach subskrypcji. Aby uzyskać więcej informacji, zobacz [Przenoszenie subskrypcji do użytkownika w innej dzierżawie usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Przenoszenie własności subskrypcji**

Przeniesienie własności subskrypcji wiąże się z utratą dostępu kontroli opartej na rolach do zarządzania zasobami w subskrypcji. Aby uzyskać więcej informacji na temat dodawania istniejącej subskrypcji do dzierżawy, zobacz [Skojarzenie lub dodanie subskrypcji platformy Azure do usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Przeniesienie subskrypcji z istniejącą zaległą kwotą z bieżącego cyklu rozliczeniowego nie zostanie przeniesione na nowy środek płatniczy na nowym koncie. Jedyną informacją dostępną dla użytkowników na nowym koncie jest koszt subskrypcji w ostatnim miesiącu. Pozostała część historii użycia i rozliczeń nie jest przenoszona razem z subskrypcją.
- Przenoszenie własności rozliczeń subskrypcji Enterprise Agreement jest obecnie obsługiwane wyłącznie w portalu Enterprise Agreement
- Przeniesienie subskrypcji opartej na środkach (np. Visual Studio, BizSpark, Microsoft Partner Network) na nowego użytkownika wymaga licencji programu Visual Studio/Microsoft Partner Network, aby zaakceptować żądanie przeniesienia.
- Wszystkie zasoby, takie jak maszyny wirtualne, dyski i witryny internetowe, zostaną pomyślnie przeniesione na nowe konto. Przeniesienie subskrypcji między dzierżawami może mieć wpływ na następujące zasoby:

Usługi **Azure AD Domain Services**

Azure Key Vault

- Może to mieć wpływ na [użytkowników i bazy danych powiązane z usługą SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support), zwłaszcza jeśli klient korzysta z uwierzytelniania powiązanego z usługą Azure Active Directory.
- Może to mieć wpływ na **usługi aplikacji**, które są skonfigurowane do uwierzytelniania przy użyciu usługi Azure Active Directory
- Konta usług **Visual Studio Team Services** połączone z subskrypcjami platformy Azure mogą tymczasowo utracić dostęp, gdy połączona subskrypcja platformy Azure zostanie anulowana.

**Zalecane dokumenty**

Kroki po zaakceptowaniu własności rozliczeń:

- Aby zachować własność rozliczeń, ale zmienić typ subskrypcji, zobacz: [Przełączanie subskrypcji platformy Azure do innej oferty](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Przenoszenie subskrypcji programu Visual Studio, witryny Microsoft Partner Network (MPN) oraz płatności zgodnie z rzeczywistym użyciem podczas tworzenia/testowania](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Przenoszenie własności rozliczeń subskrypcji Enterprise Agreement](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Przenoszenie własności — często zadawane pytania](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Rozwiązywanie problemów dotyczących przenoszenia własności](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
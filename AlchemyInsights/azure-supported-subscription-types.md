---
title: Obsługiwane typy abonamentów
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807975"
---
# <a name="supported-subscription-types"></a>Obsługiwane typy abonamentów

Sprawdź Obsługiwane typy abonamentów, aby kontynuować.

[Obsługiwane typy abonamentów](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Przeniesienie własności do rozliczeń**

Portal Azure jako [administrator konta](https://ms.portal.azure.com/) konta rozliczeniowego z subskrypcją, którą chcesz przenieść

- Wyszukaj w obszarze **Zarządzanie kosztami + rozliczenia** . Wybierz pozycję **subskrypcje** z okienka po lewej stronie. W zależności od dostępu może być konieczne wybranie zakresu rozliczeń, a następnie **abonamentów** lub **subskrypcji platformy Azure** .
- Wybieranie prawa własności do rozliczeń dla subskrypcji, którą chcesz przenieść
- Wprowadź adres e-mail użytkownika, który jest administratorem rozliczeń konta, który będzie nowym właścicielem subskrypcji, a następnie wybierz pozycję **Wyślij żądanie przeniesienia**
- Użytkownik otrzyma wiadomość e-mail z instrukcjami w celu przejrzenia żądania przeniesienia. Aby zatwierdzić żądanie przeniesienia, użytkownik wybiera link w wiadomości e-mail i postępuje zgodnie z instrukcjami.

Uwaga: Jeśli przekierujesz własność rozliczeniową abonamentu na konto użytkownika w innej dzierżawie usługi Azure AD, wszystkie przydziały [kontroli dostępu oparte na rolach (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) do zarządzania zasobami w ramach subskrypcji zostaną trwale usunięte. Tylko nowy właściciel będzie miał dostęp do zarządzania zasobami w ramach subskrypcji. Aby uzyskać więcej informacji, zobacz [przenoszenie subskrypcji do użytkownika w innej dzierżawie usługi Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Przenoszenie własności subskrypcji**

Prawo własności abonamentu — wymagania wstępne dostęp roli (RBAC) do zarządzania zasobami w ramach abonamentu tracą dostęp. Aby uzyskać więcej informacji na temat dodawania istniejącej subskrypcji do dzierżawy, zobacz [kojarzenie lub Dodawanie subskrypcji platformy Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Przeniesienie subskrypcji z istniejącą kwotą zaległą z bieżącego cyklu rozliczeniowego nie będzie przenoszona do nowego instrumentu płatniczego na nowym koncie. Jedyne informacje dostępne dla użytkowników w nowym koncie to koszt ostatniego miesiąca abonamentu. Pozostała część historii użytkowania i rozliczeń nie jest przekazywana razem z subskrypcją.
- Prawa własności do rozliczania z rozliczeniami w programie Enterprise Agreement (EA) są obecnie obsługiwane tylko w portalu Enterprise Agreement
- Przeniesienie abonamentu związanego z doładowaniem, takiego jak Visual Studio, BizSpark, sieci partnerskiej firmy Microsoft do nowego użytkownika wymaga posiadania licencji sieciowej programu Visual Studio/partnera firmy Microsoft w celu zaakceptowania żądania przeniesienia.
- Wszystkie zasoby, takie jak maszyny wirtualne, dyski i witryny internetowe, są przesyłane pomyślnie do nowego konta. W ramach transferu abonamentu między dzierżawcami mogą być narażone następujące zasoby:

**Usługi domenowe w usłudze Azure AD**

Magazyny kluczy Azure

- Może to wpłynąć na [pokrewnych użytkowników i bazy danych SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) , szczególnie jeśli klient korzysta z uwierzytelniania powiązanego z usługą Azure Active Directory
- Może mieć wpływ na **usługi aplikacji** skonfigurowane przy użyciu uwierzytelniania usługi Azure Active Directory
- **Program Visual Studio Team** Konta usług powiązane z subskrypcjami platformy Azure mogą tymczasowo utracić dostęp, gdy połączona subskrypcja platformy Azure zostanie anulowana

**Polecane dokumenty**

Kroki po zaakceptowaniu własności do rozliczeń:

- Aby zachować własność rozliczeniową, ale zmienić typ abonamentu, zobacz: [przełączanie subskrypcji platformy Azure do innej oferty](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Przenoszenie programu Visual Studio, sieci partnera firmy Microsoft (MPN) i regulowanie abonamentów na dev/testowe](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Przeniesienie własności do rozliczania abonamentów umowy Enterprise (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Przekazywanie praw własności — często zadawane pytania](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Rozwiązywanie problemów dotyczących przekazywania własności](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
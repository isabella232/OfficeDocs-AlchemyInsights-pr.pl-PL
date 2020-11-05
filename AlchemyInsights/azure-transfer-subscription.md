---
title: Transferowanie własności usługi Azure do rozliczeń
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922165"
---
# <a name="transfer-azure-billing-ownership"></a>Transferowanie własności usługi Azure do rozliczeń

Zaloguj się w [witrynie Azure Portal](https://portal.azure.com/) jako administrator konta rozliczeniowego z subskrypcją, którą chcesz przenieść. Jeśli nie masz pewności, czy jesteś administratorem, lub jeśli potrzebujesz określić, kto jest, zobacz [Określanie administratora rozliczania kont](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Wyszukaj w obszarze **Zarządzanie kosztami + rozliczenia**.
- Wybierz pozycję **subskrypcje** z okienka po lewej stronie. W zależności od dostępu może być konieczne wybranie zakresu rozliczeń, a następnie **abonamentów** lub **subskrypcji platformy Azure**.
- Wybieranie **prawa własności do rozliczeń** dla subskrypcji, którą chcesz przenieść
- Wprowadź adres e-mail użytkownika, który jest administratorem rozliczeń konta, który będzie nowym właścicielem subskrypcji, a następnie wybierz pozycję **Wyślij żądanie przeniesienia**
- Użytkownik otrzyma wiadomość e-mail z instrukcjami w celu przejrzenia żądania przeniesienia. Aby zatwierdzić żądanie przeniesienia, użytkownik wybiera link w wiadomości e-mail i postępuje zgodnie z instrukcjami.

**Uwaga** : Jeśli przekierujesz własność rozliczeniową abonamentu na konto użytkownika w innej dzierżawie usługi Azure AD, wszystkie przydziały [kontroli dostępu oparte na rolach (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)do zarządzania zasobami w ramach subskrypcji zostaną trwale usunięte. Tylko nowy właściciel będzie miał dostęp do zarządzania zasobami w ramach subskrypcji. Aby uzyskać więcej informacji, zobacz [przenoszenie subskrypcji do użytkownika w innej dzierżawie usługi Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Polecane dokumenty**

- [Prawo do przenoszenia prawa własności do konta usługi Azure na innym koncie](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Informacje o transferowaniu własności do rozliczeń dla subskrypcji platformy Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Przenoszenie programu Visual Studio, sieci partnera firmy Microsoft (MPN) i regulowanie abonamentów na dev/testowe](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Przekazywanie praw własności — często zadawane pytania](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Rozwiązywanie problemów dotyczących przekazywania własności](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)

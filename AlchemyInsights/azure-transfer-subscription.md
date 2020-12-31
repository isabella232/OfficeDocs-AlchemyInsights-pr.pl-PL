---
title: Przenoszenie własności rozliczeń platformy Azure
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
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736888"
---
# <a name="transfer-azure-billing-ownership"></a>Przenoszenie własności rozliczeń platformy Azure

Zaloguj się do portalu [Azure Portal](https://portal.azure.com/) jako administrator konta rozliczeniowego z subskrypcją, którą chcesz przenieść. Jeśli nie masz pewności, czy jesteś administratorem usługi, lub, jeśli chcesz określić, kto nim jest, zobacz [Określanie administratora rozliczeń kont](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Szukaj w pozycji _Zarządzanie kosztami + rozliczenia_.
1. Wybierz pozycję **Subskrypcje** z okienka po lewej stronie. W zależności od dostępu może być konieczne wybranie zakresu rozliczeń, a następnie pozycji **Subskrypcje** lub **Subskrypcje platformy Azure**.
1. Wybierz pozycję **Przenieś własność rozliczeń** dla subskrypcji, którą chcesz przenieść.
1. Wprowadź adres e-mail użytkownika, który jest administratorem rozliczeń konta, które będzie nowym właścicielem subskrypcji, a następnie wybierz pozycję **wyślij żądanie przeniesienia**.
1. Użytkownik otrzyma wiadomość e-mail z instrukcjami dotyczącymi rozpatrzenia żądania przeniesienia. Aby zatwierdzić żądanie przeniesienia, użytkownik wybiera link w wiadomości e-mail i postępuje zgodnie z instrukcjami.

Zwróć uwagę, że jeśli przeniesiesz własność rozliczeń subskrypcji do konta użytkownika w innej dzierżawie usługi Azure AD, wszystkie przypisania [kontroli dostępu na podstawie ról (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) do zarządzania zasobami w ramach subskrypcji zostaną trwale usunięte. Tylko nowy właściciel będzie mieć dostęp do zarządzania zasobami w ramach subskrypcji. Aby uzyskać więcej informacji na temat zmieniania katalogu subskrypcji, zobacz [Przenoszenie subskrypcji do użytkownika w innej dzierżawie usługi Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Ważny wpływ na faktury**_: jeśli chcesz przenieść własność rozliczeń subskrypcji platformy Azure, Twoje opłaty będą proporcjonalne. Będziesz mieć możliwość uzyskania dostępu do faktur za pomocą następujących metod:  

1. Wybierz swoją subskrypcję na stronie  [Subskrypcje](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) w portalu Azure Portal jako [użytkownik mający dostęp do faktur](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), a następnie wybierz pozycję **Faktury**.
1. Kliknij pozycję **Pobierz fakturę** , aby wyświetlić kopię faktury w formacie PDF. Jeśli zostanie wyświetlony komunikat _Niedostępna_, zobacz [Dlaczego nie widzę faktury za ostatni okres rozliczeniowy?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Możesz także wyświetlić dzienne użycie, klikając **okres rozliczeniowy** w celu uzyskania faktury w formacie PDF i skopiowania pliku szczegółowego dziennego użycia (CSV). Aby uzyskać więcej informacji, zobacz [Pobieranie danych faktury i użycia](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Polecane dokumenty**

- [Przenoszenie własności rozliczeń subskrypcji platformy Azure na inne konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Informacje o przenoszeniu własności rozliczeń dla subskrypcji platformy Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Przenoszenie subskrypcji programu Visual Studio, sieci Microsoft Partner Network (MPN) i płatności zgodnie z rzeczywistym użyciem podczas tworzenia/testowania](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Przenoszenie własności — często zadawane pytania](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Rozwiązywanie problemów dotyczących przenoszenia własności](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)

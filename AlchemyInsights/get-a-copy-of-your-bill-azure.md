---
title: Potrzebna kopia rachunku lub użycia
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6804"
ms.openlocfilehash: 5ec935ddd9e273561886831e60c98ae1a542f9da
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808382"
---
# <a name="get-a-copy-of-your-bill-or-usage"></a>Uzyskiwanie kopii rachunku lub użycia

**Pobierz fakturę na platformie Azure (PDF)**

1. Wybierz abonament na [stronie Subskrypcje](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) w portalu Azure Portal jako [użytkownik z dostępem do faktur](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support) , a następnie wybierz pozycję **faktury**
2. Kliknij pozycję **Pobierz fakturę** , aby wyświetlić kopię faktury w formacie PDF. Jeśli ta informacja jest **niedostępna** , zobacz [dlaczego nie jest wyświetlana faktura za ostatni okres rozliczeniowy?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
3. Możesz również wyświetlić codzienne użytkowanie, klikając okres rozliczeniowy, aby uzyskać plik PDF faktury i kopię szczegółowego codziennego pliku użytkowania (. CSV): [pobieranie danych dotyczących faktur i użycia](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)

**Pobierz fakturę w wiadomości e-mail (PDF)**

1. Wybierz abonament na [stronie Subskrypcje](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade). Kliknij pozycję **faktury** , a następnie **Wyślij fakturę**
2. Kliknij pozycję **Zrezygnuj** i zaakceptuj warunki. W przypadku każdej abonamentu trzeba będzie to zrobić. Uwaga: Jeśli po wykonaniu tych czynności nie otrzymasz wiadomości e-mail, upewnij się, że Twój adres e-mail jest prawidłowy w [preferencjach komunikacji w profilu](https://account.windowsazure.com/profile) .
3. [Faktury w usłudze Azure są wysyłane bezpośrednio do skrzynki odbiorczej](https://azure.microsoft.com/blog/azure-email-invoices/)

**Opis codziennego użytkowania:**  
 [Opis rachunku na platformie Microsoft Azure](https://docs.microsoft.com/azure/cost-management-billing/understand/review-individual-bill?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Zarządzanie kosztami:** [zapobieganie nieoczekiwanym kosztom w ramach zarządzania rozliczeniami i kosztami usługi Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/getting-started?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Umowa z klientami firmy Microsoft (MCA)** :

Dowiedz się  [, jak sprawdzić dostęp do umowy z klientem firmy Microsoft?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)  
Jeśli korzystasz z [umowy Microsoft Customer](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement), możesz pobrać użycie w [witrynie Azure Portal](https://portal.azure.com/)

**Uzyskiwanie faktur w ramach umów dotyczących klientów firmy Microsoft w wiadomości e-mail** :

Jeśli masz umowę z klientem firmy Microsoft, możesz skorzystać z listy, aby otrzymać fakturę w wiadomości e-mail. Wszyscy właściciele profilów rozliczeń, współautorzy, czytelnicy i menedżerowie faktur otrzymają fakturę pocztą e-mail. Czytelnicy nie mogą zaktualizować preferencji dotyczących faktury e-mail

- Wyszukaj **Zarządzanie kosztami + rozliczenia** . Wybierz pozycję **profil rozliczeniowy** . W obszarze Ustawienia wybierz pozycję **Właściwości**
- W obszarze faktura za wiadomość E-mail wybierz pozycję **Aktualizuj preferencję na fakturze e-mail** . Wybierz pozycję Zrezygnuj. Kliknij pozycję **Aktualizuj**

**Umowa Enterprise (EA)**

Aby wyświetlić i pobrać dane dotyczące użycia jako klienta z atrybutem EA, musisz być administratorem przedsiębiorstwa, właścicielem konta lub administratorem działu z włączonymi zasadami "Wyświetl opłaty".

- Zaloguj się w witrynie Azure Portal. Wyszukaj **Zarządzanie kosztami + rozliczenia** . Wybierz profil rozliczeń
- Wybierz pozycję użycie + opłaty. Dla miesiąca, który chcesz pobrać, wybierz pozycję Pobierz.

**Abonament na platformie MOSP Azure**  
[Pobierz fakturę za subskrypcję usługi Azure MOSP](https://docs.microsoft.com/azure/cost-management-billing/understand/download-azure-invoice?WT.mc_id=Portal-Microsoft_Azure_Support#download-your-mosp-azure-subscription-invoice)

**Rozwiązywanie problemów: nie można wyświetlić faktury za ostatni okres rozliczeniowy?**

Niektóre z możliwych powodów, na które może nie być widoczna faktura:

- Masz miesięczną kwotę doładowania abonamentu, którego nie przekroczyłeś lub że masz bezpłatny okres próbny. Faktura jest generowana tylko w przypadku zadłużenia pieniędzy
- To mniej niż 30 dni od dnia, w którym subskrybujesz usługę Azure
- Faktura nie została jeszcze wygenerowana. Poczekaj na zakończenie okresu rozliczeniowego
- Jeśli nie jesteś administratorem konta, starsze faktury mogą być niedostępne dla Ciebie **Uwaga** : Firma Microsoft nie udostępnia żadnych raportów użycia ani danych dotyczących zużycia użytkownikom usług dostawcy CSP platformy Azure. Dane użycia Centrum partnerskiego są oparte na partnerach
- Dowiedz się więcej na temat rozliczeń i użytkowania usługi AIO (Azure in Open): [Azure w usłudze Open](https://azure.microsoft.com/offers/ms-azr-0111p/)

**Polecane dokumenty**

- [Dlaczego faktura może nie być widoczna?](https://docs.microsoft.com/azure/cost-management-billing/understand/download-azure-invoice?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
- [Żądanie/pobieranie/wyświetlanie danych na fakturze rozliczeniowej na platformie Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Jak wysłać pocztą e-mail faktury na platformie Azure bezpośrednio do skrzynki odbiorczej](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis szczegółowych opłat za użycie](https://docs.microsoft.com/azure/cost-management-billing/understand/review-individual-bill?WT.mc_id=Portal-Microsoft_Azure_Support#csv)
- [Opis warunków na fakturze](https://docs.microsoft.com/azure/cost-management-billing/understand/understand-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis faktury usług kryptograficznych na platformie Azure](https://docs.microsoft.com/partner-center/azure-plan-lp?WT.mc_id=Portal-Microsoft_Azure_Support)

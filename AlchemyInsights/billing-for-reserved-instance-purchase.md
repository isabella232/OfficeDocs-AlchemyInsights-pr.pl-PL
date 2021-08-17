---
title: Rozliczanie zakupu Reserved Instance
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104030"
---
# <a name="billing-for-reserved-instance-purchase"></a>Rozliczanie zakupu Reserved Instance

Zakup Reserved Instance jest rozliczany przy użyciu metody płatności powiązanej z subskrypcją, która jest wybierana w momencie dokonywania zakupu. Typ subskrypcji musi być umową typu enterprise (numer oferty: MS-AZR-0017P), Pay-As-You-Go (numer oferty: MS-AZR-0003P), Umową z Klientem Microsoft lub Microsoft Cloud Solution Provider.

- W przypadku subskrypcji przedsiębiorstwa opłaty są odliczane od salda zobowiązania pieniężnego rejestracji lub pobierane na zasadzie nadwyżki
- W przypadku subskrypcji Pay-As-You-Go opłaty są pobierane z karty płatniczej lub za pomocą metody płatności faktury w ramach subskrypcji

**Anulowanie rezerwacji**

- **Samoobsługa:** możesz anulować lub wymienić wystąpienie zarezerwowane korzystając z portalu [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Wybierz rezerwację i kliknij opcję zwrotu kosztów lub wymiany. Zauważ, że aby można było dokonać wymiany lub otrzymać zwrot kosztów, musisz mieć dostęp do zamówienia rezerwacji jako właściciel. Sam dostęp do rezerwacji nie umożliwia zwrotu kosztów ani wymiany. Poproś właściciela zamówienia rezerwacji o nadanie Ci dostępu do zamówienia rezerwacji
- **Zasady wymiany:** możesz zmienić rezerwację na rezerwację tego samego typu. Za wymianę rezerwacji nie są naliczane **żadne kary**. Całkowita kwota zobowiązania za nową rezerwację powinna być większa niż suma zwrotu kosztów wymienianej rezerwacji i przyszłych rat miesięcznych (jeśli mają zastosowanie)
- **Zasady zwrotu kosztów:** suma zwrotu i anulowanych przyszłych płatności nie może przekroczyć w okresie 12 miesięcy 50 000 USD. **Obecnie nie naliczamy żadnych kar** za zwroty, ale możemy naliczać je w przyszłości.

**Wyjątki:** funkcja samoobsługowej wymiany i anulowania nie jest dostępna dla klientów programu US Government Enterprise Agreement

- W przypadku anulowania i zwrotu kosztów w ramach [Samoobsługowej wymiany i zwrotu kosztów w usłudze Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) nie jest dostępna pomoc techniczna dla **API/PS/CLI**
- Funkcja samoobsługowej wymiany i anulowania nie jest dostępna dla klientów programu US Government Enterprise Agreement. Obsługiwane są inne subskrypcje amerykańskich instytucji rządowych, w tym płatność zgodnie z rzeczywistym użyciem i program Microsoft Cloud Solution Provider

Dowiedz się więcej: [Jak są przetwarzane transakcje](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) zwrotów i wymiany Dowiedz się [więcej:](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Exchange i Zasady zwrotu kosztów Inne pytania: Odwiedź [zarezerwowane dokumenty wystąpień](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Wymiana istniejącego wystąpienia zarezerwowanego (samoobsługa)**

Możesz wymienić rezerwację na inną rezerwację tego samego typu. Możesz również otrzymać zwrot kosztów rezerwacji, jeśli nie jest już potrzebna, w wysokości do 50 000 USD rocznie. Funkcja samoobsługowej wymiany i anulowania nie jest dostępna dla klientów programu US Government Enterprise Agreement. Obsługiwane są inne subskrypcje amerykańskich instytucji rządowych, w tym płatność zgodnie z rzeczywistym użyciem i program Microsoft Cloud Solution Provider. Aby można było dokonać wymiany lub otrzymać zwrot kosztów, musisz mieć dostęp do zamówienia rezerwacji jako właściciel.

Poniższe kroki przedstawiają procedurę realizacji transakcji

1.Zaloguj się do [portalu Azure Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Wybierz rezerwacje, które chcesz zwrócić, i kliknij pozycję Exchange  2.Wybierz produkt maszyny wirtualnej, który chcesz kupić, i wpisz liczbę. Upewnij się, że nowa suma zakupu jest większa niż suma zwrotu [Określ odpowiedni rozmiar przed zakupem](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Przejrzyj i ukończ transakcję

**Zwrot kosztów wystąpienia zarezerwowanego**

Aby otrzymać zwrot kosztów za rezerwację, przejdź do obszaru **Szczegóły rezerwacji** i kliknij przycisk **Zwrot**

**Proporcjonalny zwrot kosztów:**

**Pro-ration i przykłady minimalnych wymagań w przypadku zwrotu i wymiany** Przykład rezerwacji z góry:

- 1 stycznia kupujesz RI na jeden rok za 120 USD
- 7 kwietnia chcesz zmienić rezerwację lub otrzymać zwrot kosztów
- Ponieważ rezerwacja była aktywna przez 97 dni, otrzymasz zwrot o wartości (1-97/365) * 120 USD. (czyli 88,1 USD). Obecnie nie naliczamy żadnych kar za zwroty
- W przypadku wymiany wartość nowego zakupu powinna być większa niż 88,1 USD.
- Obecnie nie naliczamy żadnych kar za zwroty

**Przykład planu rozliczeniowego rezerwacji:**

- Wykupujesz RI na jeden rok za 10 USD miesięcznie
- 7 kwietnia chcesz zmienić rezerwację lub otrzymać zwrot kosztów
- Ponieważ ostatnia płatność miała miejsce 7 dni temu, otrzymasz zwrot o wartości (1-7/31) * 10 USD. (czyli 7,74 USD).
- Przyszłe anulowane płatności to 80 USD. Obecnie nie naliczamy żadnych kar za zwroty
- To anulowanie spowoduje odliczenie 87,74 USD od kwoty 50 000 USD limitu zwrotu
- W przypadku wymiany całkowita wartość nowego zakupu powinna być większa niż 87,74 USD.

**Nie można wyświetlić faktury za ostatni okres rozliczeniowy**

Niektóre możliwe przyczyny mogą nie być wyświetlanie faktury:

- Masz miesięczną kwotę środków na koncie w ramach subskrypcji, która nie została przekroczona lub że masz bezpłatną wersję próbną. Faktura jest generowana tylko wtedy, gdy masz należne pieniądze
- Minie mniej niż 30 dni od dnia subskrybowania platformy Azure
- Faktura nie została jeszcze wygenerowana. Poczekaj do końca okresu rozliczeniowego
- Jeśli nie jesteś administratorem konta, starsze faktury mogą być niedostępne

**Pobierz fakturę z portalu Azure Portal (.pdf)**

- Wybierz swoją subskrypcję na [stronie Subskrypcje w](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Portalu Azure jako [użytkownik z dostępem do faktur](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Wybierz **pozycję Faktury**
- Kliknij **pozycję Pobierz fakturę,** aby wyświetlić kopię faktury PDF. Jeśli jest **dostępna,** zobacz Dlaczego nie widzę faktury [za ostatni okres rozliczeniowy?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Otrzymywanie faktury w wiadomości e-mail (.pdf)**

- Wybierz swoją subskrypcję na [stronie Subskrypcje.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Kliknij **pozycję Faktury, a** następnie wyślij fakturę pocztą e-mail
- Kliknij **pozycję przysyłaj** i zaakceptuj warunki. Musisz wybrać każdą posiadaną subskrypcję

Uwaga: Jeśli po zakończeniu procedury nie otrzymasz wiadomości e-mail, upewnij się, że Twój adres e-mail jest poprawny w preferencjach [komunikacji w Twoim profilu](https://account.windowsazure.com/profile)

**Pobieranie danych dotyczących użycia z portalu Azure Portal**

- Zaloguj się do [Centrum kont Azure](https://account.windowsazure.com/Subscriptions) jako administrator [konta](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Wybierz subskrypcję, dla której chcesz uzyskać fakturę i informacje dotyczące użycia
- Wybierz **pozycję Historia rozliczeń**
- Wybierz **pozycję Wyświetl bieżące zestawienie,** aby wyświetlić szacowaną opłatę w momencie wygenerowania szacowania
- Wybierz **pozycję Pobierz użycie,** aby pobrać codzienne dane użycia jako plik CSV. Jeśli są dostępne dwie wersje, pobierz wersję 2

Inne pytania: [Zapoznaj się z dokumentacją na temat wystąpienia zarezerwowanego](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zalecane dokumenty**

- [Podstawy rozliczeń](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis sposobu stosowania rabatu na zarezerwowane wystąpienie](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Pobieranie lub wyświetlanie danych dotyczących codziennego użycia i faktur rozliczeniowych usługi Azure](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis sposobu stosowania rabatu na zarezerwowane wystąpienie](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis użycia zarezerwowanego wystąpienia dla subskrypcji usługi Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis użycia zarezerwowanego wystąpienia dla rejestrowania Enterprise danych](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows koszty oprogramowania nieujmowane w wystąpieniach zastrzeżonych](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Zarezerwowane wystąpienia w centralnym programie Dostawca rozwiązań w chmurze partnerów (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)
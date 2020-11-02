---
title: Rozliczenia zarezerwowane na zakup wystąpienia zastrzeżonego
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
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823165"
---
# <a name="billing-for-reserved-instance-purchase"></a>Rozliczenia zarezerwowane na zakup wystąpienia zastrzeżonego

Zastrzeżony zakup jest naliczany według metody płatności powiązanej z subskrypcją wybraną w momencie zakupu. Typem abonamentu musi być Umowa Enterprise (Numer oferty: MS-AZR-0017P), płać na bieżąco (Numer oferty: MS-AZR-0003P), umowa lub dostawca usług Microsoft Customer.

- W przypadku abonamentu w przedsiębiorstwie opłaty są odejmowane od pieniężnego salda zobowiązań w ramach rejestracji lub naliczana jako nieprzekraczająca
- W przypadku abonamentu płatne za opłatą za opłatą naliczana jest opłata za kartę kredytową lub metodę płatności faktury w ramach abonamentu.

**Anulowanie rezerwacji**

- Samoobsługowe **:** Możesz anulować lub zastanowić zastrzeżoną instancję samodzielnie za pomocą [portalu Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Wybierz rezerwację i kliknij pozycję zwrot kosztów lub Exchange. Zwróć uwagę, że w zamówieniu rezerwacji musisz mieć dostęp właściciela do wymiany lub zwrotu pieniędzy. Dostęp tylko do tej rezerwacji nie pozwala na kontynuowanie zwrotu pieniędzy lub wymiany. Poproś właściciela zamówienia rezerwacji o udzielenie użytkownikowi dostępu do zamówienia rezerwacji.
- **Zasady programu Exchange:** Rezerwację można wymienić na inną rezerwację tego samego typu — **nie ma kar** za wymianę rezerwacji. Całkowite zobowiązanie z nową rezerwacją powinno być większe niż suma kwot zwrotu i przyszłych płatności miesięcznych (jeśli dotyczy)
- **Zasady dotyczące zwrotów:** Suma zwrotu i anulowane płatności przyszłe nie mogą przekroczyć $50 000 USD w 12-miesięcznym oknie kroczącym. **Obecnie nie ładujemy żadnych kar** za refundacje, ale mogą naliczać opłaty za przyszłe refundacje

**Wyjątki:** Możliwość samodzielnej wymiany i anulowania funkcji jest niedostępna dla klientów kontraktowych w Stanach Zjednoczonych dla przedsiębiorstw

- Obsługa **interfejsu API/PS/CLI** jest niedostępna w przypadku anulowania i zwrotu kosztów [samodzielnej wymiany i zwrotów za rezerwacje usługi Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Możliwość samodzielnej wymiany i funkcji anulowania nie jest dostępna dla klientów kontraktowych w Stanach Zjednoczonych dla przedsiębiorstw. Obsługiwane są inne typy abonamentów publicznych w Stanach Zjednoczonych, w tym z opcją Płać na bieżąco i dostawcę CSP

Dowiedz się więcej: [jak transakcje zwrotu i wymiany są przetwarzane](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) więcej informacji: [usługi Exchange i zasady dotyczące zwrotów](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) — inne pytania: [odwiedź dokumenty zastrzeżonych wystąpień](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Wymienia istniejące zarezerwowane wystąpienie (samoobsługowe)**

Rezerwację można wymienić na inną rezerwację tego samego typu. Możesz również zwrócić zastrzeżenie, do $50 000 USD rocznie, jeśli nie jest już potrzebne. Możliwość samodzielnej wymiany i funkcji anulowania nie jest dostępna dla klientów kontraktowych w Stanach Zjednoczonych dla przedsiębiorstw. Obsługiwane są inne typy abonamentów w Stanach Zjednoczonych, w tym z opcją Płać na bieżąco i dostawcę CSP. Aby móc wymieniać lub refundować istniejące zastrzeżenie, użytkownik musi mieć dostęp właściciela w zamówieniu rezerwacji.

Poniższe czynności pozwolą na wykonanie procedury realizacji transakcji.

1. Zaloguj się w usłudze [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Wybierz rezerwacje, które chcesz zwrócić, i kliknij pozycję **Exchange** 2. Wybierz produkt maszynowy, który chcesz kupić, i wpisz ilość. Upewnij się, że suma zakupów jest większa niż suma zwrotu, [zanim zaczniesz kupować](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. Sprawdź i Ukończ transakcję.

**Zwrot kosztów za zastrzeżone wystąpienie**

Aby zwrócić zastrzeżenie, przejdź do **szczegółów zastrzeżenia** i kliknij pozycję **zwrot kosztów** .

**Pro proporcjonalna kwota:**

**Pakiet Pro-racja i minimalne wymagania dotyczące wymagań dotyczących zwrotu kosztów i wymiany** Przykład rezerwacji przedniej:

- Kupisz jednoletni okres RI dla $120 r. 1 stycznia
- 7 kwietnia, które chcesz refundować lub wymienić to zastrzeżenie
- Ze względu na to, że rezerwacja była na bieżąco przez 97 dni, będziesz otrzymywać (1-97/365) * $120. (na przykład $88,1). Obecnie nie ma żadnych kar za refundacje
- W przypadku wymiany nowy zakup powinien być większy niż $88,1
- Obecnie nie są dostępne żadne kary za refundacje

**Przykładowa rezerwacja planu rozliczeń:**

- Po zakupie jednoletniego okresu RI na $10 miesięcznie
- 7 kwietnia, które chcesz refundować lub wymienić to zastrzeżenie
- Od momentu dokonania ostatniej płatności w ciągu 7 dni otrzymasz (1-7/31) * $10 wstecz. (tzn. $7,74)
- Anulowane przyszłe płatności to $80. Obecnie nie ma żadnych kar za refundacje
- To anulowanie spowoduje odjęcie $87,74 od Ciebie limitu refundacji $50 000
- W przypadku wymiany, łączna wartość nowego zakupu powinna być większa niż $87,74

**Nie można wyświetlić faktury za ostatni okres rozliczeniowy**

Niektóre z możliwych powodów, na które może nie być widoczna faktura:

- Masz miesięczną kwotę doładowania abonamentu, którego nie przekroczyłeś lub że masz bezpłatny okres próbny. Faktura jest generowana tylko w przypadku zadłużenia pieniędzy
- To mniej niż 30 dni od dnia, w którym subskrybujesz usługę Azure
- Faktura nie została jeszcze wygenerowana. Poczekaj na zakończenie okresu rozliczeniowego
- Jeśli nie jesteś administratorem konta, starsze faktury mogą nie być dostępne.

**Pobierz fakturę z portalu Azure (plik PDF)**

- Wybierz abonament na stronie [subskrypcje](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) w portalu Azure Portal jako [użytkownik z dostępem do faktur](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Wybieranie **faktur**
- Kliknij pozycję **Pobierz fakturę** , aby wyświetlić kopię faktury w formacie PDF. Jeśli ta informacja jest **niedostępna** , zobacz [dlaczego nie jest wyświetlana faktura za ostatni okres rozliczeniowy?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Odbieranie faktury w wiadomości e-mail (PDF)**

- Wybierz abonament na stronie [subskrypcje](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Kliknij pozycję **faktury** , a następnie Wyślij fakturę
- Kliknij pozycję **Zrezygnuj** i zaakceptuj warunki. Musisz wybrać dla każdej subskrypcji

Uwaga: Jeśli po wykonaniu tych czynności nie otrzymasz wiadomości e-mail, upewnij się, że Twój adres e-mail jest prawidłowy w [preferencjach komunikacji w profilu](https://account.windowsazure.com/profile) .

**Pobieranie danych użycia z portalu Azure**

- Logowanie się do [centrum konta platformy Azure](https://account.windowsazure.com/Subscriptions) jako [administratora konta](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Wybierz subskrypcję, dla której chcesz uzyskać informacje o fakturze i użyciu.
- Wybierz **historię rozliczeń**
- Wybierz pozycję **Wyświetl bieżącą instrukcję** , aby zobaczyć szacowaną opłatę w chwili generowania oszacowania
- Wybierz pozycję **Pobierz użycie** , aby pobrać codzienne dane dotyczące użycia jako plik CSV. Jeśli zobaczysz dwie dostępne wersje, Pobierz wersję 2

Inne pytania: [odwiedź dokumenty zastrzeżonych wystąpień](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Polecane dokumenty**

- [Podstawowe informacje dotyczące rozliczeń](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis sposobu stosowania rabatu zarezerwowanego dla wystąpienia](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Pobieranie lub wyświetlanie faktury za rozliczanie na platformie Azure oraz codzienne dane dotyczące użycia](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis sposobu stosowania rabatu zarezerwowanego dla wystąpienia](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis sposobu użycia zarezerwowanych dla abonamentu Płać na bieżąco](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis zastosowania zarezerwowanych wystąpień rejestracji w przedsiębiorstwie](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Koszty oprogramowania systemu Windows nie są objęte zarezerwowanymi wystąpieniami](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Zastrzeżone wystąpienia w programie partnerskim centralnym rozwiązaniem w chmurze (CSP) partnera](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)
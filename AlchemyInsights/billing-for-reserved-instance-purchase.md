---
title: Rozliczenia za zakup zarezerwowanego wystąpienia
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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820332"
---
# <a name="billing-for-reserved-instance-purchase"></a>Rozliczenia za zakup zarezerwowanego wystąpienia

Zakup zarezerwowanego wystąpienia jest obciążony metodą płatności powiązaną z subskrypcją, która została wybranych w momencie zakupu. Typ subskrypcji musi być umową dla przedsiębiorstw (numer oferty: MS-AZR-0017P), płatnością na czas użytkownika (numer oferty: MS-AZR-0003P), Umową klienta firmy Microsoft lub CSP.

- W przypadku subskrypcji dla przedsiębiorstw opłaty są odejmowane z salda zobowiązania pieniężnego rejestracji lub naliczane jako zamówienie
- W przypadku subskrypcji usługi Pay-As-You-Go opłaty są rozliczane na podstawie karty kredytowej lub metody płatności za pomocą faktury w subskrypcji

**Anulowanie rezerwacji**

- **Samoobsługowa:** Możesz anulować lub wymienić zarezerwowane wystąpienie samodzielnie za pomocą [Portalu Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Wybierz rezerwację i kliknij przycisk zwrotu kosztów lub wymiany. Pamiętaj, że aby dokonać wymiany lub zwrotu kosztów, musisz mieć dostęp właściciela w zamówieniu rezerwacji. Dostęp tylko do rezerwacji nie umożliwia kontynuowania zwrotu ani wymiany. Poproś właściciela zamówienia rezerwacji o nadanie Ci dostępu do zamówienia rezerwacji
- **Zasady programu Exchange:** Możesz zmienić rezerwację na inną rezerwację tego  samego typu — nie ma żadnych wątpliwości w sprawie rezerwacji. Całkowita kwota zobowiązania z nową rezerwacją powinna być większa niż suma zwrotu kosztów rezerwacji oraz przyszłych płatności miesięcznych (jeśli ma zastosowanie)
- **Zasady zwrotu kosztów:** Suma zwrotu kosztów i anulowane przyszłe płatności nie mogą przekroczyć 50 000 USD w 12-miesięcznym oknie. Obecnie nie **obciążamy żadnych** kosztów zwrotów, ale możemy obciążyć je przyszłych zwrotami kosztów.

**Wyjątki:** Funkcja samoobsługowej wymiany i anulowania nie jest dostępna dla klientów programu US Government Enterprise Agreement

- **Anulowanie i zwroty** kosztów za samoobsługowe wymiany i zwroty kosztów za rezerwacje Azure nie są dostępne w przypadku obsługi interfejsu API/ps/interfejsu [obsługi klienta](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Funkcja samoobsługowej wymiany i anulowania nie jest dostępna dla klientów programu US Government Enterprise Agreement. Inne typy subskrypcji dla instytucji rządowych Stanów Zjednoczonych, w tym płatności zgodnie z płatnością i program CSP, są obsługiwane

Dowiedz się więcej: [Jak są przetwarzane transakcje zwrotów](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) i wymiany Dowiedz się więcej: Zasady programu [Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) i Zwrotu kosztów Inne pytania: Odwiedź [zarezerwowane dokumenty wystąpienia](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange an existing reserved instance (Self-service)**

Możesz zmienić rezerwację na inną rezerwację tego samego typu. Możesz również zwrócić rezerwację w wysokości do 50 000 USD rocznie, jeśli nie jest już potrzebna. Funkcja samoobsługowej wymiany i anulowania nie jest dostępna dla klientów programu US Government Enterprise Agreement. Inne typy subskrypcji dla instytucji rządowych Stanów Zjednoczonych, w tym płatności zgodnie z płatnością i programem CSP, są obsługiwane. Aby można było wymienić lub zwrócić istniejącą rezerwację, musisz mieć dostęp właściciela do zamówienia rezerwacji.

Poniższe kroki poszukaj procedury ukończenia transakcji.

1.Zaloguj się do [portalu Azure Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Wybierz rezerwacje, które chcesz zwrócić, a następnie kliknij pozycję **Exchange** 2.Wybierz produkt maszyny wirtualnej, który chcesz kupić, i wpisz liczbę. Upewnij się, że nowa suma zakupu jest większa niż suma zwrotu [Określ odpowiedni rozmiar przed zakupem](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Przejrzyj i ukończ transakcję

**Zwrot kosztów za zarezerwowane wystąpienie**

Aby zwrócić kosztów rezerwacji, przejdź do **szczegółów rezerwacji i** kliknij pozycję **Zwrot kosztów.**

**Zwrot proporcjonalny:**

**Przykłady wymaganych pro racji i minimalnych wymagań w celu zwrotu kosztów i wymiany** Przykład rezerwacji z góry:

- 1 stycznia zakupisz 1-letni okres RI za 120 ZŁ
- 7 kwietnia chcesz zwrócić lub wymienić tę rezerwację
- Ponieważ rezerwacja jest żywa przez 97 dni, otrzymasz (1-97/365) * 120 USD wstecz. (czyli 88,1 zł). Obecnie nie ma żadnych opłat za zwrot kosztów
- W przypadku wymiany nowy zakup powinien być większy niż 88,1 USD
- Obecnie nie ma żadnych opłat za zwrot kosztów

**Przykład rezerwacji planu rozliczeniowego:**

- Zakup 1-okresowego RI za 10 USD miesięcznie
- 7 kwietnia chcesz zwrócić lub wymienić tę rezerwację
- Od ostatniej płatności nastąpiło 7 dni, otrzymasz (1-7/31) * 10 zł wstecz. (to jest 7,74 zł)
- Przyszłe anulowane płatności w wysokości 80 ZŁ. Obecnie nie ma żadnych opłat za zwrot kosztów
- To anulowanie odejmuje 87,74 zł od limitu zwrotu 50 000 zł
- W przypadku wymiany łączna wartość nowego zakupu powinna być większa niż 87,74 USD.

**Nie można wyświetlić faktury za ostatni okres rozliczeniowy**

Niektóre możliwe przyczyny mogą nie być wyświetlanie faktury:

- Masz miesięczną kwotę środków na koncie w ramach subskrypcji, która nie została przekroczona lub że masz bezpłatną wersję próbną. Faktura jest generowana tylko wtedy, gdy masz należne pieniądze
- Minie mniej niż 30 dni od dnia subskrybowania platformy Azure
- Faktura nie została jeszcze wygenerowana. Poczekaj do końca okresu rozliczeniowego
- Jeśli nie jesteś administratorem konta, starsze faktury mogą być niedostępne

**Pobierz fakturę z portalu Azure Portal (pdf)**

- Wybierz swoją subskrypcję na [stronie Subskrypcje w](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Portalu Azure jako [użytkownik z dostępem do faktur](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Wybierz **pozycję Faktury**
- Kliknij **pozycję Pobierz fakturę,** aby wyświetlić kopię faktury PDF. Jeśli jest **dostępna,** zobacz Dlaczego nie widzę faktury [za ostatni okres rozliczeniowy?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Otrzymywanie faktury w wiadomości e-mail (pdf)**

- Wybierz swoją subskrypcję na [stronie Subskrypcje.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Kliknij **pozycję Faktury, a** następnie wyślij fakturę pocztą e-mail
- Kliknij **pozycję przysyłaj** i zaakceptuj warunki. Musisz wybrać każdą posiadaną subskrypcję

Uwaga: Jeśli po zakończeniu procedury nie otrzymasz wiadomości e-mail, upewnij się, że Twój adres e-mail jest poprawny w preferencjach [komunikacji w Twoim profilu](https://account.windowsazure.com/profile)

**Pobieranie danych dotyczących użycia z portalu Azure Portal**

- Zaloguj się do [Centrum kont Azure](https://account.windowsazure.com/Subscriptions) jako administrator [konta](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Wybierz subskrypcję, dla której chcesz uzyskać fakturę i informacje dotyczące użycia
- Wybierz **pozycję Historia rozliczeń**
- Wybierz **pozycję Wyświetl bieżące zestawienie,** aby wyświetlić szacowaną opłatę w momencie wygenerowania szacowania
- Wybierz **pozycję Pobierz użycie,** aby pobrać codzienne dane użycia jako plik CSV. Jeśli są dostępne dwie wersje, pobierz wersję 2

Inne pytania: [Odwiedź zarezerwowane dokumenty wystąpień](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Polecane dokumenty**

- [Podstawy rozliczeń](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis sposobu stosowania rabatu na zarezerwowane wystąpienie](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Pobieranie lub wyświetlanie danych dotyczących codziennego użycia i faktur rozliczeniowych usługi Azure](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis sposobu stosowania rabatu na zarezerwowane wystąpienie](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis użycia zarezerwowanego wystąpienia dla subskrypcji usługi Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Opis użycia zarezerwowanego wystąpienia dla rejestracji przedsiębiorstwa](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Koszty oprogramowania systemu Windows, które nie są uwzględnione w wystąpieniach zastrzeżonych](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Zarezerwowane wystąpienia w programie CSP (Partner Central Cloud Solution Provider)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)
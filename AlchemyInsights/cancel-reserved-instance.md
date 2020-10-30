---
title: Anulowanie rezerwacji
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807994"
---
# <a name="cancelling-reservation"></a>Anulowanie rezerwacji

- Samoobsługowe **:** Możesz anulować lub zastanowić zastrzeżoną instancję samodzielnie za pomocą [portalu Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Wybierz rezerwację i kliknij pozycję zwrot kosztów lub Exchange. Zwróć uwagę, że w zamówieniu rezerwacji musisz mieć dostęp właściciela do wymiany lub zwrotu pieniędzy. Dostęp tylko do tej rezerwacji nie pozwala na kontynuowanie zwrotu pieniędzy lub wymiany. Poproś właściciela zamówienia rezerwacji o udzielenie użytkownikowi dostępu do zamówienia rezerwacji.
- **Zasady programu Exchange:** Rezerwację można wymienić na inną rezerwację tego samego typu — **nie ma kar** za wymianę rezerwacji. Całkowite zobowiązanie z nową rezerwacją powinno być większe niż suma kwot zwrotu i przyszłych płatności miesięcznych (jeśli dotyczy)
- **Zasady dotyczące zwrotów:** Suma zwrotu i anulowane płatności przyszłe nie mogą przekroczyć $50 000 USD w 12-miesięcznym oknie kroczącym. **Obecnie nie ładujemy żadnych kar** za refundacje, ale mogą naliczać opłaty za przyszłe refundacje  
    **Wyjątki:** Możliwość samodzielnej wymiany i anulowania funkcji jest niedostępna dla klientów kontraktowych w Stanach Zjednoczonych dla przedsiębiorstw
- Obsługa **interfejsu API/PS/CLI** jest niedostępna w przypadku anulowania i zwrotu kosztów [samodzielnej wymiany i zwrotów za rezerwacje usługi Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Możliwość samodzielnej wymiany i funkcji anulowania nie jest dostępna dla klientów kontraktowych w Stanach Zjednoczonych dla przedsiębiorstw. Obsługiwane są inne typy abonamentów publicznych w Stanach Zjednoczonych, w tym z opcją Płać na bieżąco i dostawcę CSP

Dowiedz się więcej: [sposób przetwarzania transakcji zwrotu i wymiany](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Dowiedz się więcej: [zasady programu Exchange i zwrot kosztów](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Inne pytania: [odwiedź dokumenty zastrzeżonych wystąpień](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Wymienia istniejące zarezerwowane wystąpienie (samoobsługowe)**

Rezerwację można wymienić na inną rezerwację tego samego typu. Możesz również zwrócić zastrzeżenie, do $50 000 USD rocznie, jeśli nie jest już potrzebne. Możliwość samodzielnej wymiany i funkcji anulowania nie jest dostępna dla klientów kontraktowych w Stanach Zjednoczonych dla przedsiębiorstw. Obsługiwane są inne typy abonamentów w Stanach Zjednoczonych, w tym z opcją Płać na bieżąco i dostawcę CSP. Aby móc wymieniać lub refundować istniejące zastrzeżenie, użytkownik musi mieć dostęp właściciela w zamówieniu rezerwacji.

Poniższe czynności pozwolą na wykonanie procedury realizacji transakcji.

1. Zaloguj się w [witrynie Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Wybierz rezerwacje, które chcesz refundować, a następnie kliknij pozycję **Exchange** .
2. Wybierz produkt MASZYNowy, który chcesz kupić, a następnie wpisz ilość. Upewnianie się, że suma zakupów jest większa niż suma zwrotu, [przed zakupem należy określić odpowiedni rozmiar](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy) .
3. Przeglądanie i Kończenie transakcji

**Zwrot kosztów za zastrzeżone wystąpienie**

Aby zwrócić zastrzeżenie, przejdź do **szczegółów zastrzeżenia** i kliknij pozycję **zwrot kosztów** .

**Pro proporcjonalna kwota:**

**Pakiet Pro-racja i minimalne wymagania dotyczące wymagań dotyczących zwrotu kosztów i wymiany**  
Przykład rezerwacji przedniej:

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

**Polecane dokumenty**

- [Sposób przetwarzania transakcji zwrotu i wymiany](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Zasady programu Exchange i zwrot kosztów](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)
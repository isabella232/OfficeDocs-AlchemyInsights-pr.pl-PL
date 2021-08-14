---
title: Anulowanie rezerwacji
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
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931243"
---
# <a name="cancelling-reservation"></a>Anulowanie rezerwacji

- **Samoobsługa:** możesz anulować lub wymienić wystąpienie zarezerwowane korzystając z portalu [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Wybierz rezerwację i kliknij opcję zwrotu kosztów lub wymiany. Zauważ, że aby można było dokonać wymiany lub otrzymać zwrot kosztów, musisz mieć dostęp do zamówienia rezerwacji jako właściciel. Sam dostęp do rezerwacji nie umożliwia zwrotu kosztów ani wymiany. Poproś właściciela zamówienia rezerwacji o nadanie Ci dostępu do zamówienia rezerwacji
- **Zasady wymiany:** możesz zmienić rezerwację na rezerwację tego samego typu. Za wymianę rezerwacji nie są naliczane **żadne kary**. Całkowita kwota zobowiązania za nową rezerwację powinna być większa niż suma zwrotu kosztów wymienianej rezerwacji i przyszłych rat miesięcznych (jeśli mają zastosowanie)
- **Zasady zwrotu kosztów:** suma zwrotu i anulowanych przyszłych płatności nie może przekroczyć w okresie 12 miesięcy 50 000 USD. **Obecnie nie naliczamy żadnych kar** za zwroty, ale możemy naliczać je w przyszłości.  
    **Wyjątki:** funkcja samoobsługowej wymiany i anulowania nie jest dostępna dla klientów programu US Government Enterprise Agreement
- W przypadku anulowania i zwrotu kosztów w ramach [Samoobsługowej wymiany i zwrotu kosztów w usłudze Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) nie jest dostępna pomoc techniczna dla **API/PS/CLI**
- Funkcja samoobsługowej wymiany i anulowania nie jest dostępna dla klientów programu US Government Enterprise Agreement. Obsługiwane są inne subskrypcje amerykańskich instytucji rządowych, w tym płatność zgodnie z rzeczywistym użyciem i program Microsoft Cloud Solution Provider

Więcej informacji: [Przetwarzanie transakcji zwrotu kosztów i wymiany](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Więcej informacji: [Zasady wymiany i zwrotu kosztów](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Inne pytania: [Zapoznaj się z dokumentacją na temat wystąpienia zarezerwowanego](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Wymiana istniejącego wystąpienia zarezerwowanego (samoobsługa)**

Możesz wymienić rezerwację na inną rezerwację tego samego typu. Możesz również otrzymać zwrot kosztów rezerwacji, jeśli nie jest już potrzebna, w wysokości do 50 000 USD rocznie. Funkcja samoobsługowej wymiany i anulowania nie jest dostępna dla klientów programu US Government Enterprise Agreement. Obsługiwane są inne subskrypcje amerykańskich instytucji rządowych, w tym płatność zgodnie z rzeczywistym użyciem i program Microsoft Cloud Solution Provider. Aby można było dokonać wymiany lub otrzymać zwrot kosztów, musisz mieć dostęp do zamówienia rezerwacji jako właściciel.

Poniższe kroki przedstawiają procedurę realizacji transakcji

1. Zaloguj się do portalu [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Wybierz rezerwacje, za które chcesz otrzymać zwrot kosztów, i kliknij przycisk **Wymiana**
2. Wybierz produkt maszyny wirtualnej, który chcesz kupić, a następnie wpisz ilość. Upewnij się, że całkowita wartość nowego zakupu jest większa niż kwota zwrotu [Ustal odpowiedni rozmiar przed zakupem](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Przejrzyj i zakończ transakcję

**Zwrot kosztów wystąpienia zarezerwowanego**

Aby otrzymać zwrot kosztów za rezerwację, przejdź do obszaru **Szczegóły rezerwacji** i kliknij przycisk **Zwrot**

**Proporcjonalny zwrot kosztów:**

**Przykłady zastosowania proporcjonalności i wymagań minimalnych dla zwrotu kosztów i wymiany**  
Przykład rezerwacji z wyprzedzeniem:

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

**Zalecane dokumenty**

- [Przetwarzanie transakcji zwrotu kosztów i wymiany](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Zasady wymiany i zwrotu kosztów](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)
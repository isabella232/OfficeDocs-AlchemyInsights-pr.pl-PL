---
title: Dlaczego przycisk Dodaj budżet jest dla mnie wyłączony?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822645"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Dlaczego przycisk Dodaj budżet jest dla mnie wyłączony?

Aby utworzyć budżet, potrzebujesz jednej z następujących uprawnień:

- Grupa zarządzania, Subskrypcja, Zakresy grup zasobów
- Współautor zarządzania kosztami
- Właściciel
- Współautor
- Tylko dla klientów w przedsiębiorstwie: Rejestracja, Dział, Zakresy kont
- Administrator rejestracji (ustaw budżet w zakresie rejestracji)
- Administrator działu (ustaw budżet w zakresie Dział)
- Właściciel konta (ustaw budżet w zakresie Klienta)
- Tylko nowoczesne umowy klienta: Konto rozliczeniowe, Profil rozliczeniowy, Zakresy sekcji faktury
- Kreator subskrypcji platformy Azure

**Budżet został utworzony, gdy koszt dla bieżącego miesiąca już został u mnie zaoczny. Dlaczego nie otrzymałem alertu?**  
Jeśli po utworzeniu budżetu już przekroczono próg kosztów, alert nie zostanie ostrzegany. Gdy rozpocznie się nowy cykl, w przypadku naruszenia progu alert zostanie ostrzegany.

**Kiedy mam oczekiwać otrzymywania alertu po przekroczeniu jednego z moich zdefiniowanych progów alertów budżetowych?**  
Budżety są obliczane co 4 godziny. Docieranie danych dotyczących użycia do systemu budżetów trwa co najmniej 8 godzin. W związku z tym alerty mogą być zwalniane nawet przez 12 godzin po przekroczeniu progu.

**Dlaczego przycisk Data rozpoczęcia jest wyłączony po wybraniu okresu resetowania Miesiąc lub Miesiąc rozliczeniowy?**  
Budżety są zgodne z bieżącym miesiącem kalendarzowym lub bieżącym okresem rozliczeniowym (w przypadku, gdy wybrano miesiąc rozliczeniowy). Dlatego tę wartość jest wstępnie wypełniana.

**Dlaczego w czasie tworzenia budżetu nie widzę wykresu kosztów?**  
Aby pomóc Ci w tworzeniu budżetu, potrzebujemy co najmniej 2 miesięcy danych kosztowych, aby można było renderować wykres.

**Dlaczego nie mogę ustawić budżetu dla właśnie utworzonej subskrypcji?**  
Po utworzeniu subskrypcji przetwarzanie danych trwa 24–48 godzin, zanim zostanie na nie ustawiany budżet.

**Zasoby interfejsu API budżetu**

- [Interfejs API budżetów w wersji 1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)Udostępnia operacje tworzenia i aktualizowania budżetów. Za pomocą interfejsu API Budżety można ustawić próg budżetu i skonfigurować wiele alertów tak, aby alerty zwalniały się w granicach progu. Alerty mogą wyzwalać wiadomość e-mail lub grupę akcji platformy Azure w celu wykonania automatyzacji. Uwaga: Filtrowanie dla tego interfejsu API nie jest zgodne z filtrowaniem/wymiarami interfejsu API zapytań.
- [Interfejs API budżetów w wersji 2.](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Tworzenie budżetów z większą możliwością filtrowania kosztów niż wersja 1. Filtrowanie jest zgodne z umową używaną w naszych interfejsach API zapytań i wymiarów. Jest to zalecany interfejs API budżetów do użytku w przyszłości.
- [Wymiary:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Zapewnia operacje w celu uzyskania obsługiwanych wymiarów Twojego użycia w różnych zakresach. Za pomocą interfejsu API wymiarów można pobrać listę wymiarów, które mogą być używane jako dane wejściowe do generowania zapytań za pomocą interfejsu API zapytania.
- [Zapytanie:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Umożliwia wykonywanie operacji na celu uzyskania zagregowanych danych dotyczących kosztów i użycia na podstawie zapytania, które podano. Za pomocą interfejsu API zapytania możesz określić żądane filtrowanie, sortowanie i grupowanie we wszystkich dostępnych wymiarach (dostępnych z interfejsu API wymiarów).

**Koszty prognozowane**

**Dlaczego nie widzę prognoz dla moich kosztów w analizie kosztów?**  
Istnieje wiele powodów, dla których może brakować projekcji prognozy w analizie kosztów. Niektóre z nich są następujące:

1. Jeśli dane kosztowe są mniejsze niż 10 dni, wykres prognozy nie zostanie załadowany. Model wymaga co najmniej 10 dni ostatnich danych kosztowych dla dokładnych projekcji
2. Jeśli wybrano daty historyczne, wykres prognozy nie będzie widoczny. Wybierz zakres dat z datami przyszłymi, aby wyświetlić wykres prognozy
3. Jeśli Twoje konto ma wiele walut, wykres prognozy będzie kosztami projektu tylko dla "Wszystkich kosztów w DOLARACH"

**Dlaczego prognoza nie zmienia się, gdy wprowadzam zmiany w zasobach?**  
Model prognozy wymaga kilku dni na uwzględnianie zmian na koncie i nie przewiduje natychmiastowych prognoz na podstawie zmian w zasobach  
W przypadku większych etapów zwiększenia lub zmniejszenia ilości zasobów model będzie nieco dłużej dostosowywany do tych zmian w przypadku anomalii

**Dlaczego moja prognoza rośnie po dokonaniu rezerwacji lub zakupu w witrynie Marketplace?**  
Model prognozy uwzględnia "Koszt rzeczywisty" i nie uwzględnia użycia ani zakupu oddzielnie. W przypadku zakupu godzina model zmniejszy projekcje po 10 dniach, co spowoduje niespodziewanie wzrost kosztów

**Chcę zobaczyć prognozy dla pojedynczego wymiaru (np. Metr)**  
Prognoza obecnie obsługuje projekcje całkowitych kosztów, a nie poszczególnych metrów. Dlatego w przypadku "grupowania według" wymiaru projekcje będą na sumę wszystkich elementów w wymiarze.

**Zalecane dokumenty**

- [Co to jest usługa Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najlepsze rozwiązania dotyczące zarządzania kosztami platformy Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizowanie kosztów i wydatków](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Eksplorowanie i analizowanie kosztów za pomocą analizy kosztów](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Ceny](https://azure.microsoft.com/services/cost-management/#pricing)
- [Przeglądanie kosztów w analizie kosztów](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Samouczek wideo: tworzenie budżetu w portalu Azure Portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Wymagania wstępne dotyczące wyświetlania i dostosowywania budżetów](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Tworzenie budżetów i zarządzanie nimi](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurowanie automatyzacji za pomocą grup akcji platformy Azure i interfejsu API budżetów](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Monitorowanie użycia i wydatków za pomocą alertów o kosztach](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najlepsze rozwiązania dotyczące zarządzania kosztami](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Samouczki wideo**

- [Tworzenie budżetu w portalu Azure Portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Zarządzanie kosztami przy użyciu interfejsu API Budżety i grup akcji](https://go.microsoft.com/fwlink/?linkid=2147038)
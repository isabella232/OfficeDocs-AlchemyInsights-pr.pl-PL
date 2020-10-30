---
title: Dlaczego przycisk Dodaj budżet jest dla mnie wyłączony?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807665"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Dlaczego przycisk Dodaj budżet jest dla mnie wyłączony?

Do utworzenia budżetu wymagane jest jedno z następujących uprawnień:

- Grupa zarządzania, subskrypcja, zakresy grup zasobów
- Współautor zarządzania kosztami
- Właściciela
- Trybu
- Tylko klient w przedsiębiorstwie: Rejestracja, dział, zakresy kont
- Administrator rejestracji (Ustawianie budżetu w zakresie rejestracji)
- Administrator działu (Ustawianie budżetu w zakresie działu)
- Właściciel konta (Ustawianie budżetu w zakresie kont)
- Tylko nowoczesny kontrakt klienta: konto rozliczeniowe, profil rozliczeń, zakresy sekcji faktury
- Kreator subskrypcji platformy Azure

**Budżet został utworzony, gdy koszt w bieżącym miesiącu już przekroczył budżet. Dlaczego nie otrzymałeś alertu?**  
Jeśli przekroczenie określonego progu kosztu podczas tworzenia budżetu nie będzie wyzwalane. Po rozpoczęciu nowego cyklu, jeśli zostanie naruszony próg, zostanie wyświetlony alert.

**Kiedy należy oczekiwać, że jest wyświetlany alert po przekroczeniu jednego z zdefiniowanych progów alertów budżetu?**  
Budżety są oceniane co 4 godziny. W celu uzyskania dostępu do systemu budżetowego dane dotyczące użycia są co najmniej 8 godzin. Po przekroczeniu progu alerty mogą trwać nawet 12 godzin.

**Dlaczego przycisk Data rozpoczęcia jest wyłączony po wybraniu okresu resetowania miesięcy lub miesięcy rozliczeniowych?**  
Budżety są wyrównane do bieżącego miesiąca w kalendarzu lub bieżącego okresu rozliczeniowego (w przypadku wybrania miesiąca rozliczeniowego). W związku z tym, wstępnie wypełniam tę wartość.

**Dlaczego nie widzę wykresu kosztów w ramach funkcji tworzenia budżetu?**  
Potrzebujemy co najmniej 2 miesięcy danych kosztów, zanim będzie można renderować wykres, aby pomóc Ci w tworzeniu budżetu.

**Dlaczego nie mogę ustawić budżetu na właśnie utworzoną subskrypcję?**  
Po utworzeniu subskrypcji dane są przetwarzane na 24-48 godzin przed ustawieniem budżetu.

**Zasoby dotyczące budżetu API**

- Funkcje [budżetowe — interfejs API V1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): zawiera operacje umożliwiające tworzenie i aktualizowanie budżetów. Korzystając z interfejsu API budżety, można ustawić próg budżetu i skonfigurować wiele alertów, aby były uruchamiane po osiągnięciu tego progu. Alerty mogą wyzwolić wiadomość e-mail lub grupę akcji platformy Azure w celu wykonania automatyzacji. Uwaga: filtrowanie dla tego interfejsu API nie jest wyrównane za pomocą filtrowania/wymiarów API kwerendy.
- [Interfejs API budżetu v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Tworzenie budżetów za pomocą większej liczby funkcji filtrowania kosztów niż wersja v1. Filtrowanie powoduje wyrównanie do umowy używanej w kwerendach i interfejsach API dotyczących zapytań i wymiarów. Jest to zalecany interfejs API dla budżetu, który umożliwia przenoszenie do przodu.
- [Wymiary](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): zawiera funkcje umożliwiające korzystanie z obsługiwanych wymiarów dla korzystania z różnych zakresów. Korzystając z interfejsu API Dimensions, można pobrać listę wymiarów, które mogą być używane jako dane wejściowe dla generowania zapytań za pomocą interfejsu API zapytania.
- [Kwerenda](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): umożliwia wykonywanie operacji uzyskiwania zagregowanych danych dotyczących kosztu i użycia na podstawie dostarczonych zapytań. Korzystając z interfejsu API kwerendy, możesz określić żądane filtrowanie, sortowanie i grupowanie we wszystkich dostępnych wymiarach (do których można uzyskać dostęp z interfejsu API Dimensions).

**Prognozowane koszty**

**Dlaczego nie widzę prognoz kosztów w analizie kosztów?**  
Istnieje wiele powodów, dla których projekcja prognozy w analizie kosztów może być brakująca, niektóre z nich są następujące:

1. Jeśli dane o kosztach są starsze niż 10 dni, wykres prognozy nie zostanie załadowany. Model wymaga co najmniej 10 dni ostatnich danych dotyczących kosztów, aby uzyskać dokładne prognozowanie
2. Jeśli wybrano daty historyczne, wykres prognozy nie będzie widoczny. Wybierz zakres dat z przyszłymi datami wyświetlania wykresu prognozy.
3. Jeśli na Twoim koncie jest wiele walut, wykres prognozy będzie uwzględniać tylko koszty wszystkich kosztów w USD.

**Dlaczego Prognoza nie zmienia się po wprowadzeniu zmian w moich zasobach?**  
Model prognozy wymaga kilku dni na uwzględnienie zmian na koncie i nie dokonuje bezpośrednich prognoz na podstawie zmian w zasobach  
W przypadku większych kroków zwiększania lub zmniejszania zasobów model zajmie nieco więcej czasu, dostosowując się do tych zmian pod kątem anomalii.

**Dlaczego moja Prognoza wzrasta po dokonaniu rezerwacji lub zakupieniu w witrynie Marketplace?**  
Model prognozy uwzględnia swój "koszt rzeczywisty" i nie uwzględnia zakupów oddzielnie. W przypadku zakupu jednorazowego model obniży prognozę po 10 dniach, aby uwzględnić nagły wzrost kosztów.

**Chcę wyświetlić prognozy dla pojedynczego wymiaru (np. Miernik**  
Prognoza obsługuje obecnie prognozy kosztów całkowitych, a nie dla poszczególnych liczników. Stąd też, gdy wymiar "pogrupowany według" jest sumą wszystkich elementów w wymiarze

**Polecane dokumenty**

- [Co to jest zarządzanie kosztami platformy Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najważniejsze wskazówki dotyczące zarządzania kosztami na platformie Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizowanie kosztów i wydatków](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Eksplorowanie i analizowanie kosztów za pomocą analizy kosztów](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Zarządzanie kosztami na platformie Azure: Cennik](https://azure.microsoft.com/services/cost-management/#pricing)
- [Przegląd kosztów w analizie kosztów](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Samouczek wideo: Tworzenie budżetu w portalu Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Wymagania wstępne dotyczące wyświetlania i dostosowywania budżetów](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Tworzenie budżetów i zarządzanie nimi](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurowanie automatyzacji za pomocą interfejsu API grup akcji i budżetów platformy Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Monitorowanie użycia i wydatków za pomocą alertów dotyczących kosztów](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najważniejsze wskazówki dotyczące zarządzania kosztami](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Klipy wideo samouczka**

- [Tworzenie budżetu w portalu Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Zarządzanie kosztami za pomocą interfejsu API budżetu i grup akcji](https://go.microsoft.com/fwlink/?linkid=2147038)
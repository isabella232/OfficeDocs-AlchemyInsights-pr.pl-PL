---
title: Badanie interfejsu API programu Microsoft Graph
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974681"
---
# <a name="querying-the-microsoft-graph-api"></a>Badanie interfejsu API programu Microsoft Graph

Ten temat może również dotyczyć deweloperów korzystających z interfejsu API Azure AD Graph. Jednak **stanowczo** zaleca się korzystanie z programu Microsoft Graph we wszystkich scenariuszach dotyczących katalogów, tożsamości i zarządzania dostępem.

**Problemy z uwierzytelnianiem lub autoryzacją**

- Jeśli aplikacja **nie może uzyskać tokenów** w celu nawiązania połączenia z programem Microsoft Graph, wybierz pozycję problem, aby uzyskać bardziej szczegółową pomoc i obsługę techniczną dotyczącą tego tematu, wybierając kategorię Microsoft Graph **token (uwierzytelnianie)** .
- Jeśli aplikacja otrzymuje **Błędy autoryzacji usługi 401 lub 403** podczas nawiązywania połączenia z programem Microsoft Graph, wybierz kategorię **błąd podczas uzyskiwania dostępu** do aplikacji Microsoft Graph API, aby uzyskać bardziej właściwą pomoc i obsługę techniczną w tym temacie.

**Chcę używać programu Microsoft Graph, ale nie wiesz, gdzie zacząć**

Aby uzyskać więcej informacji na temat programu Microsoft Graph, zobacz:

- [Omówienie programu Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Omówienie zarządzania tożsamościami i dostępem w programie Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Wprowadzenie do tworzenia aplikacji Microsoft Graph](https://docs.microsoft.com/graph/)
- **Eksplorator Microsoft Graph** -testowanie interfejsów API programu Microsoft Graph w dzierżawie lub w dzierżawie demonstracyjnej

**Chcę używać programu Microsoft Graph, ale obsługuje on interfejsy API katalogów v 1.0?**

Program Microsoft Graph to zalecany interfejs API dla katalogu, tożsamości i zarządzania dostępem. Jednak w przypadku programu Azure AD Graph i Microsoft Graph nadal są dostępne niewiele przerw. Zapoznaj się z następującymi artykułami, które wyróżnią najbardziej aktualne różnice, aby pomóc w wyborze:

- [Różnice typów zasobów na platformie Azure AD Graph i w programie Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Różnice między właściwościami programu Azure AD Graph a programem Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Różnice między metodami Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Podczas wysyłania zapytania do obiektu *użytkownika* brakuje wielu jego właściwości**

`GET https://graph.microsoft.com/v1.0/users` zwraca tylko 11 właściwości, ponieważ program Microsoft Graph automatycznie wybiera domyślny zestaw właściwości *użytkownika* , które mają zostać zwrócone. Jeśli potrzebujesz innych właściwości *użytkownika* , użyj $SELECT, aby wybrać właściwości, których potrzebuje aplikacja. Najpierw wypróbuj **program Microsoft Graph Explorer** .

**Niektóre wartości właściwości użytkownika mają *wartość null* , mimo że wiemy, że są ustawione**

Najbardziej prawdopodobnym wyjaśnieniem jest to, że dla aplikacji udzielono uprawnienia *User. ReadBasic. All* . Umożliwia to aplikacji odczytywanie ograniczonego zestawu właściwości użytkownika i zwracanie wszystkich innych właściwości jako wartości null, nawet jeśli zostały one wcześniej ustawione. Spróbuj udzielić użytkownikowi aplikacji *. Przeczytaj. wszystkie* uprawnienia.

Aby uzyskać więcej informacji, zobacz [uprawnienia użytkownika programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Występują problemy z używaniem parametrów zapytania OData w celu filtrowania danych w moich żądaniach**

Gdy program Microsoft Graph obsługuje szeroki zakres parametrów zapytania OData, wiele z tych parametrów nie jest w pełni obsługiwane przez usługi katalogowe (zasoby dziedziczące po elemencie *directoryobject*) w programie Microsoft Graph. Te same ograniczenia, które były dostępne w programie Azure AD Graph, są zachowywane w większości części programu Microsoft Graph:

1. **Nieobsługiwane**: $count, $search i $Filter wartości *null* lub *not null*
2. **Nieobsługiwane**: $Filter niektórych właściwości (zobacz tematy dotyczące zasobów, na których właściwości można filtrować)
3. **Nieobsługiwane**: stronicowanie, filtrowanie i sortowanie w tym samym czasie
4. **Nieobsługiwane**: filtrowanie w relacji. Na przykład — Znajdź wszystkich członków grupy inżynierskiej w Wielkiej Brytanii.
5. **Pomoc techniczna częściowa**: $OrderBy dla *użytkownika* (DisplayName, tylko userPrincipalName) i *Group*
6. **Pomoc techniczna częściowa**: $Filter (obsługiwana tylko *w przypadku funkcji* *EQ*, *StartsWith* *lub*( *i*), $expand (rozwinięcie relacji pojedynczego obiektu zwraca wszystkie relacje, ale rozwijanie kolekcji obiektów) jest ograniczone.

Aby uzyskać więcej informacji, zobacz [Dostosowywanie odpowiedzi za pomocą parametrów kwerendy](https://docs.microsoft.com/graph/query-parameters).

**Wywołanie funkcji API nie działa — gdzie można wykonać więcej testów?**

**Eksplorator Microsoft Graph** — Przetestuj interfejsy API programu Microsoft Graph w dzierżawie lub w dzierżawie demonstracyjnej, a także zapoznaj się z **przykładowymi kwerendami** w Eksploratorze Microsoft Graph.

**Gdy badam dane, tak wygląda na to, że wybiorę niekompletny zestaw danych**

Jeśli wysyłasz zapytanie do kolekcji (na przykład *Użytkownicy*), program Microsoft Graph używa limitów stron po stronie serwera, więc wyniki są zawsze zwracane z domyślnym rozmiarem strony. Aplikacja powinna zawsze oczekiwać na przechodzenie między pozostałymi kolekcjami zwróconymi z usługi.

Aby uzyskać więcej informacji, zobacz:

- [Najważniejsze wskazówki dotyczące programu Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Stronicowanie danych programu Microsoft Graph w aplikacji](https://docs.microsoft.com/graph/paging)

**Moja aplikacja jest zbyt wolna i jest również dowolnie ograniczana. Jakie usprawnienia można wprowadzić?**

W zależności od tego, co się stanie, w dyspozycji jest wiele różnych opcji, które umożliwiają wydajniejszą realizację aplikacji, a w niektórych przypadkach jest to mniej podatne na ograniczenie działania usługi (gdy zbyt wiele połączeń).

Aby dowiedzieć się więcej, zobacz:

- [Najważniejsze wskazówki dotyczące programu Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Żądania wsadowe](https://docs.microsoft.com/graph/json-batching)
- [Śledzenie zmian za pomocą kwerendy Delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Otrzymywanie powiadomień o zmianach za pośrednictwem webhook](https://docs.microsoft.com/graph/webhooks)
- [Wskazówki dotyczące ograniczania](https://docs.microsoft.com/graph/throttling)

**Gdzie można znaleźć więcej informacji o błędach i znanych problemach?**

- [Informacje dotyczące odpowiedzi na błędy programu Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Znane problemy dotyczące programu Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Gdzie można sprawdzić dostępność statusu usługi i łączności?**

Dostępność usług i łączność podstawowych usług, do których można uzyskać dostęp za pośrednictwem programu Microsoft Graph, może wpływać na ogólną dostępność i wydajność programu Microsoft Graph.

- W przypadku kondycji usługi Azure Active Directory Sprawdź stan **zabezpieczeń + usługi tożsamości** wymienione na [stronie Stan platformy Azure](https://azure.microsoft.com/status/).
- W przypadku usług pakietu Office, które współużytkują się z programem Microsoft Graph, sprawdź stan usług wymienionych na [pulpicie nawigacyjnym kondycja usługi Office](https://portal.office.com/adminportal/home#/servicehealth).

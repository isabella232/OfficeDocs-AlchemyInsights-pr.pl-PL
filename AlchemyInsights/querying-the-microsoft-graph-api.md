---
title: Wykonywanie zapytań w interfejsie API microsoft Graph
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923249"
---
# <a name="querying-the-microsoft-graph-api"></a>Wykonywanie zapytań w interfejsie API microsoft Graph

Ten temat może również dotyczyć deweloperów, którzy nadal Graph API usługi Azure AD. Jednak zdecydowanie **zaleca** się używanie programu Microsoft Graph we wszystkich scenariuszach zarządzania katalogiem, tożsamością i dostępem.

**Problemy z uwierzytelnianiem lub autoryzacją**

- Jeśli aplikacja nie może uzyskać **tokenów** do połączenia z usługą Microsoft Graph, wybierz problem z uzyskaniem tokenu dostępu **(uwierzytelniania)** kategorii Microsoft Graph, aby uzyskać bardziej konkretną pomoc i obsługę techniczną w tym temacie.
- Jeśli podczas wywoływania aplikacji Microsoft Graph są wyświetlanych **401 lub 403** błędy autoryzacji, wybierz kategorię Interfejs API Microsoft Graph Pobieranie błędu odmówiono dostępu **(Autoryzacja),** aby uzyskać bardziej konkretną pomoc i obsługę techniczną w tym temacie.

**Chcę używać aplikacji Microsoft Graph, ale nie mam pewności, od czego zacząć**

Aby dowiedzieć się więcej o aplikacji Microsoft Graph, zobacz:

- [Omówienie aplikacji Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Omówienie zarządzania tożsamościami i dostępem w aplikacji Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Wprowadzenie do tworzenia aplikacji Microsoft Graph](https://docs.microsoft.com/graph/)
- **Eksplorator Graph Microsoft** — testowanie interfejsów API usługi Microsoft Graph w dzierżawie lub dzierżawie pokazowej

**Chcę używać aplikacji Microsoft Graph, ale czy obsługuje ona potrzebne interfejsy API katalogu w wersji 1.0?**

Microsoft Graph to zalecany interfejs API do zarządzania katalogami, tożsamościami i dostępem. Istnieje jednak nadal kilka różnic między tym, co jest możliwe w usłudze Azure AD Graph Microsoft Graph. Zapoznaj się z następującymi artykułami, w których wyróżnisz najnowsze różnice, które mogą pomóc Ci w wyborze:

- [Różnice między typami zasobów między usługami Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Różnice między właściwościami usług Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Różnice między metodami usług Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Podczas wykonywania zapytań *na obiekcie* użytkownika brakuje wielu jego właściwości**

`GET https://graph.microsoft.com/v1.0/users`zwraca tylko 11 właściwości, ponieważ program Microsoft Graph automatycznie wybiera domyślny zestaw właściwości *użytkownika* do zwrócenia. Jeśli potrzebujesz innych *właściwości użytkownika,* użyj $select właściwości aplikacji. Najpierw wypróbuj je w **Eksploratorze Graph Microsoft.**

**Niektóre wartości właściwości użytkownika mają *wartość null,* mimo że wiem, że są ustawione**

Najbardziej prawdopodobne wyjaśnienie jest to, że aplikacji udzielono uprawnienia *User.ReadBasic.All.* Dzięki temu aplikacja może odczytać ograniczony zestaw właściwości użytkownika, zwracając wszystkie inne właściwości jako wartości null, nawet jeśli zostały wcześniej ustawione. Spróbuj udzielić aplikacji *uprawnienia User.Read.All.*

Aby uzyskać więcej informacji, [zobacz Graph użytkownika usługi Microsoft](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Mam problem z używaniem parametrów zapytania OData do filtrowania danych w żądaniach**

Mimo że usługa Microsoft Graph obsługuje szeroki zakres parametrów zapytania OData, wiele z tych parametrów nie jest w pełni obsługiwanych przez usługi katalogowe (zasoby dziedziczące po *kataloguObject)* w usłudze Microsoft Graph. Te same ograniczenia, które były obecne w usłudze Azure AD Graph są zachowywane dla większości części w usłudze Microsoft Graph:

1. **Nie obsługiwane:**$count, $search i $filter wartości *null* lub *nie*
2. **Nie obsługiwane:**$filter dla niektórych właściwości (zobacz tematy zasobów dotyczące właściwości, dla których można filtrować)
3. **Nie obsługiwane:** jednocześnie: stronicowanie, filtrowanie i sortowanie
4. **Nie obsługiwane:** filtrowanie relacji. Na przykład — znajdź wszystkich członków grupy inżynierskiej, którzy znajdują się w Wielkiej Brytanii.
5. **Częściowa obsługa:**$orderby na *użytkowniku* (tylko displayName i userPrincipalName) i *grupie*
6. **Częściowa** obsługa: $filter (obsługuje tylko *eq,* *startswith* *,* lub *,* oraz , i ograniczone *dowolne)* obsługę, $expand (rozwinięcie relacji pojedynczego obiektu zwraca wszystkie relacje, ale rozszerzenie kolekcji relacji obiektów jest ograniczone)

Aby uzyskać więcej informacji, zobacz [Dostosowywanie odpowiedzi za pomocą parametrów zapytania.](https://docs.microsoft.com/graph/query-parameters)

**Interfejs API, który wołuję, nie działa — gdzie mogę wykonać więcej testów?**

**Microsoft Graph —** przetestuj interfejsy API usługi Microsoft Graph w dzierżawie  lub dzierżawie demonstracyjnej, a także zapoznaj się z przykładami zapytań w Eksploratorze Microsoft Graph.

**Gdy zapytanie dotyczące danych wygląda na to, że z powrotem zwracam niepełny zestaw danych**

Jeśli zapytanie jest zapytaniem dla kolekcji (na przykład *użytkownicy),* w aplikacji Microsoft Graph są używane limity stron po stronie serwera, więc wyniki są zawsze zwracane z domyślnym rozmiarem strony. Twoja aplikacja powinna zawsze przechodzić do stron w kolekcjach zwróconych z usługi.

Więcej informacji można znaleźć w następujących artykułach:

- [Najlepsze Graph firmy Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging Microsoft Graph danych w aplikacji](https://docs.microsoft.com/graph/paging)

**Moja aplikacja działa zbyt wolno, a ponadto jest ograniczana. Jakie ulepszenia mogę wprowadzić?**

W zależności od scenariusza twoja aplikacja ma do dyspozycji wiele różnych opcji, które sprawią, że aplikacja będzie bardziej działać, a w niektórych przypadkach będzie mniej podatna na ograniczanie jej przez usługę (kiedy wykonujesz zbyt wiele połączeń).

Aby dowiedzieć się więcej, zobacz:

- [Najlepsze Graph firmy Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Wsadowe żądania](https://docs.microsoft.com/graph/json-batching)
- [Śledzenie zmian za pomocą zapytania różnicowego](https://docs.microsoft.com/graph/delta-query-overview)
- [Otrzymuj powiadomienia o zmianach za pośrednictwem sieci Web](https://docs.microsoft.com/graph/webhooks)
- [Wskazówki dotyczące ograniczania](https://docs.microsoft.com/graph/throttling)

**Gdzie można znaleźć więcej informacji o błędach i znanych problemach?**

- [Informacje dotyczące Graph błędu w programie Microsoft](https://docs.microsoft.com/graph/errors)
- [Znane problemy dotyczące aplikacji Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Gdzie mogę sprawdzić stan dostępności i łączności usługi?**

Dostępność i łączność usług źródłowych, do których można uzyskać dostęp za pośrednictwem usługi Microsoft Graph, może mieć wpływ na ogólną dostępność i wydajność usługi Microsoft Graph.

- Aby Azure Active Directory kondycję usługi, sprawdź stan usług **Security + Identity** wymienionych na stronie stan platformy [Azure.](https://azure.microsoft.com/status/)
- Aby Office, które współtworą usługę Microsoft Graph, sprawdź stan usług wymienionych na pulpicie nawigacyjnym kondycji Office [kondycji usług.](https://portal.office.com/adminportal/home#/servicehealth)

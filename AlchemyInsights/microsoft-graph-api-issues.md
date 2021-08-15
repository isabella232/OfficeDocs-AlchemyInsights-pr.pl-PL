---
title: Problemy z interfejsem API Graph Microsoft
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
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975903"
---
# <a name="microsoft-graph-api-issues"></a>Problemy z interfejsem API Graph Microsoft

Ten temat może również dotyczyć deweloperów, którzy nadal Graph API usługi Azure AD. Jednak zdecydowanie **zaleca** się używanie programu Microsoft Graph we wszystkich scenariuszach zarządzania katalogiem, tożsamością i dostępem.

**Problemy z uwierzytelnianiem lub autoryzacją**

- Jeśli aplikacja nie może uzyskać **tokenów** do połączenia z usługą Microsoft Graph, wybierz problem z uzyskaniem tokenu dostępu **(uwierzytelniania)** kategorii Microsoft Graph, aby uzyskać bardziej konkretną pomoc i obsługę techniczną w tym temacie.
- Jeśli podczas wywoływania aplikacji Microsoft Graph są wyświetlanych **401 lub 403** błędy autoryzacji, wybierz kategorię Interfejs API Microsoft Graph Pobieranie błędu odmówiono dostępu **(Autoryzacja),** aby uzyskać bardziej konkretną pomoc i obsługę techniczną w tym temacie.

**Chcę używać aplikacji Microsoft Graph, ale nie mam pewności, od czego zacząć**

- [Omówienie aplikacji Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Omówienie zarządzania tożsamościami i dostępem w aplikacji Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Wprowadzenie do tworzenia aplikacji Microsoft Graph](https://docs.microsoft.com/graph/)
- **Eksplorator Graph Microsoft** — testowanie interfejsów API usługi Microsoft Graph w dzierżawie lub dzierżawie pokazowej

**Chcę używać aplikacji Microsoft Graph, ale czy obsługuje ona potrzebne interfejsy API katalogu w wersji 1.0?**

Microsoft Graph to zalecany interfejs API do zarządzania katalogami, tożsamościami i dostępem. Istnieje jednak nadal kilka różnic między tym, co jest możliwe w usłudze Azure AD Graph Microsoft Graph. Zapoznaj się z następującymi artykułami, w których wyróżnisz najnowsze różnice, które mogą pomóc Ci w wyborze:

- [Różnice między typami zasobów między usługami Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Różnice między właściwościami usług Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Różnice między metodami usług Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Interfejs API, który wywołuję, nie działa — gdzie mogę wykonać więcej testów?**

**Microsoft Graph —** przetestuj interfejsy API usługi Microsoft Graph w dzierżawie  lub dzierżawie demonstracyjnej, a także zapoznaj się z przykładami zapytań w Eksploratorze Microsoft Graph.

**Moja aplikacja działa zbyt wolno, a ponadto jest ograniczana. Jakie ulepszenia mogę wprowadzić?**

W zależności od scenariusza masz do dyspozycji różne opcje, które sprawią, że aplikacja będzie bardziej szkoliwa, a w niektórych przypadkach mniej podatna na ograniczenie przez usługę (kiedy wykonujesz zbyt wiele połączeń).

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

Błędy Graph autoryzacji firmy Microsoft mogą być wynikiem kilku różnych problemów, z których większość generuje błąd 401 lub 403. Na przykład do błędów autoryzacji mogą prowadzić następujące elementy:

- Nieprawidłowe [przepływy uzyskiwania tokenu dostępu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios),
- Źle skonfigurowane [zakresy uprawnień](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes),
- Brak [zgody](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent).

***Zakończenie świadczenia pomocy technicznej dla biblioteki ADAL (Azure Active Directory Authentication Library) i interfejsu API azure AD Graph (AAD Graph)***

**Począwszy od 30 czerwca 2020** r. nie będziemy już dodawać żadnych nowych funkcji do usługi ADAL ani Azure AD Graph. Będziemy nadal zapewniać pomoc techniczną i aktualizacje zabezpieczeń, natomiast nie będziemy dłużej dostarczać aktualizacji funkcji.

**Począwszy od 30 czerwca 2022 r.,** zakończymy świadczenie pomocy technicznej dla usługi ADAL i Azure AD Graph i nie będziemy już zapewniać pomocy technicznej ani aktualizacji zabezpieczeń.

Aplikacje korzystające z pliku ADAL w istniejących wersjach systemu operacyjnego będą nadal działać po tym czasie, ale nie będą korzystać z pomocy technicznej *ani aktualizacji zabezpieczeń.*

Aplikacje korzystające z usługi Azure AD Graph tym czasie mogą już nie odbierać odpowiedzi z punktu końcowego usługi Azure AD Graph sieci Web.

**Migracja ADAL**

Zalecamy zaktualizowanie do [Biblioteki uwierzytelniania Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), która oferuje najnowsze aktualizacje funkcji i zabezpieczeń.

Jeśli korzystasz z aplikacji firmy Microsoft, migruj aplikacje do programu MSAL do terminu zakończenia świadczenia pomocy technicznej, upewniając się, że będą one korzystać z bieżących ulepszeń zabezpieczeń i funkcji programu MSAL.

1. [Przeczytaj sekcję ADAL — często zadawane pytania](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Dowiedz się na temat sposobu migracji aplikacji zależnie od platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jeśli potrzebujesz pomocy w zrozumieniu, które z Twoich aplikacji korzystają z pliku ADAL, zalecamy zapoznanie się ze wszystkimi kodami źródłowymi aplikacji i, jeśli to konieczne, spływaj do wszystkich usługodawców internetowych (ISV) lub dostawców aplikacji. Pomoc techniczna firmy Microsoft może również dostarczyć listę aplikacji ADAL innych firm w Twojej dzierżawie.

**Migracja usługi AAD Graph**

W przypadku aplikacji korzystających z usługi Azure AD Graph postępuj zgodnie z naszymi wskazówkami na temat migrowania aplikacji usługi [Azure AD Graph do usługi Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Nasz lista kontrolna dotycząca migracji stanowi punkt umożliwiający rozpoczęcie](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Portal rejestracji aplikacji Azure pokazuje, jakie aplikacje używają usługi AAD Graph. Zalecamy przejrzenie kodu źródłowego wszystkich Twoich aplikacji i, w razie potrzeby, skontaktowanie się z dowolnym dostawcą ISV lub dostawcą aplikacji. Pomoc techniczna firmy Microsoft może także udostępnić listę wszystkich funkcji AAD Graph użycia w Twojej dzierżawie.
3. Aby Twoja aplikacja uzyskać dostęp do danych w aplikacji Microsoft Graph, użytkownik lub administrator musi udzielić im właściwych uprawnień w ramach procesu zgody. Odwołanie [do Graph firmy Microsoft](https://docs.microsoft.com/graph/permissions-reference) zawiera listę uprawnień skojarzonych z każdym głównym zestawem interfejsów API usługi Microsoft Graph API. Zawiera również wskazówki dotyczące korzystania z tych uprawnień.

---
title: Problemy z interfejsem API programu Microsoft Graph
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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714155"
---
# <a name="microsoft-graph-api-issues"></a>Problemy z interfejsem API programu Microsoft Graph

Ten temat może również dotyczyć deweloperów nadal korzystających z interfejsu API usługi Azure AD Graph. Jednak zdecydowanie **zalecane** jest używanie programu Microsoft Graph we wszystkich scenariuszach zarządzania katalogami, tożsamościami i dostępem.

**Problemy z uwierzytelnianiem lub autoryzacją**

- Jeśli Twoja aplikacja nie może uzyskać **tokenów** do połączenia z programem Microsoft Graph, wybierz problem z uzyskaniem kategorii tokenu dostępu **(uwierzytelniania)** programu Microsoft Graph, aby uzyskać bardziej konkretną pomoc i obsługę techniczną w tym temacie.
- Jeśli podczas wywoływania funkcji Microsoft Graph w aplikacji są wyświetlanych **401 lub 403** błędy autoryzacji, wybierz kategorię Interfejs API Microsoft Graph **(Autoryzacja),** aby uzyskać bardziej konkretną pomoc i obsługę techniczną w tym temacie.

**Chcę używać programu Microsoft Graph, ale nie wiem, od czego zacząć**

- [Omówienie programu Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Omówienie zarządzania tożsamościami i dostępem w programie Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Wprowadzenie do tworzenia aplikacji Microsoft Graph](https://docs.microsoft.com/graph/)
- **Eksplorator programu Microsoft Graph** — testowanie interfejsów API programu Microsoft Graph w dzierżawie lub dzierżawie pokazowej

**Chcę używać programu Microsoft Graph, ale czy obsługuje ono potrzebne interfejsy API katalogu w wersji 1.0?**

Microsoft Graph to zalecany interfejs API do zarządzania katalogami, tożsamościami i dostępem. Jednak nadal istnieje kilka różnic między tym, co jest możliwe w usłudze Azure AD Graph i programie Microsoft Graph. Zapoznaj się z następującymi artykułami, w których podano najbardziej aktualne różnice, które mogą pomóc Ci w wyborze:

- [Różnice między typami zasobów między programem Azure AD Graph a programem Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Różnice właściwości między programem Azure AD Graph a programem Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Różnice w metodach między usługami Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Interfejs API, do którego dzwonię, nie działa — gdzie mogę wykonać więcej testów?**

**Eksplorator Microsoft Graph** — przetestuj interfejsy API programu Microsoft Graph w dzierżawie lub dzierżawie pokazowej, a także zapoznaj się z przykładami zapytań **w** Eksploratorze programu Microsoft Graph.

**Moja aplikacja działa zbyt wolno i jest również ograniczana. Jakie ulepszenia mogę wprowadzić?**

W zależności od scenariusza masz do dyspozycji różne opcje, dzięki którym Twoja aplikacja będzie bardziej działać, a w niektórych przypadkach będzie mniej podatna na ograniczanie przez usługę (gdy wykonujesz zbyt wiele połączeń).

- [Microsoft Graph : najlepsze rozwiązania](https://docs.microsoft.com/graph/best-practices-concept)
- [Żądania wsadowe](https://docs.microsoft.com/graph/json-batching)
- [Śledzenie zmian za pomocą zapytania różnicowego](https://docs.microsoft.com/graph/delta-query-overview)
- [Otrzymuj powiadomienia o zmianach za pośrednictwem witryny internetowej](https://docs.microsoft.com/graph/webhooks)
- [Wskazówki dotyczące ograniczania](https://docs.microsoft.com/graph/throttling)

**Gdzie można znaleźć więcej informacji o błędach i znanych problemach?**

- [Informacje dotyczące odpowiedzi na błędy programu Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Znane problemy dotyczące programu Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Gdzie mogę sprawdzić stan dostępności usługi i łączności?**

Dostępność usług i łączność usług źródłowych, do których można uzyskać dostęp za pośrednictwem programu Microsoft Graph, może mieć wpływ na ogólną dostępność i wydajność programu Microsoft Graph.

- Aby sprawdzić kondycję usługi Azure Active Directory, sprawdź stan usług **Security + Identity** wymienionych na stronie stanu platformy [Azure.](https://azure.microsoft.com/status/)
- W przypadku usług pakietu Office, które współtworą program Microsoft Graph, sprawdź stan usług wymienionych na pulpicie [nawigacyjnym kondycji usług pakietu Office.](https://portal.office.com/adminportal/home#/servicehealth)

Błędy autoryzacji programu Microsoft Graph mogą być wynikiem kilku różnych problemów, z których większość generuje błąd 401 lub 403. Na przykład poniższe informacje mogą prowadzić do błędów autoryzacji:

- Nieprawidłowe [przepływy uzyskiwania tokenu dostępu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios),
- Źle skonfigurowane [zakresy uprawnień](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes),
- Brak [zgody](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent).

**_Zakończenie świadczenia pomocy technicznej dla biblioteki Azure Active Directory Authentication Library (ADAL) oraz interfejsu API usługi Azure AD Graph (AAD Graph)_* _

_*Począwszy od 30 czerwca 2020 r.**, nie będziemy już dodawać żadnych nowych funkcji do funkcji ADAL i Azure AD Graph. Będziemy nadal zapewniać pomoc techniczną i aktualizacje zabezpieczeń, natomiast nie będziemy dłużej dostarczać aktualizacji funkcji.

**Począwszy od 30 czerwca 2022 r.,** zakończymy świadczenie pomocy technicznej dla funkcji ADAL i Azure AD Graph i nie będziemy już zapewniać pomocy technicznej ani aktualizacji zabezpieczeń.

Aplikacje korzystające z pliku ADAL w istniejących wersjach systemu operacyjnego będą nadal działać po tym czasie, ale nie będą otrzymać żadnych aktualizacji pomocy technicznej ani *zabezpieczeń.*

Aplikacje korzystające z funkcji Azure AD Graph po tym czasie mogą już nie otrzymywać odpowiedzi z punktu końcowego usługi Azure AD Graph.

**Migracja ADAL**

Zalecamy zaktualizowanie do [Biblioteki uwierzytelniania Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), która oferuje najnowsze aktualizacje funkcji i zabezpieczeń.

Jeśli korzystasz z aplikacji firmy Microsoft, wiesz, że firma Microsoft jest w trakcie migrowania jej aplikacji do programu MSAL do terminu zakończenia świadczenia pomocy technicznej, aby zapewnić, że będą one korzystać z bieżących ulepszeń zabezpieczeń i funkcji pakietu MSAL.

1. [Przeczytaj sekcję ADAL — często zadawane pytania](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Dowiedz się na temat sposobu migracji aplikacji zależnie od platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jeśli potrzebujesz pomocy w zrozumieniu, które z Twoich aplikacji używają plików ADAL, zalecamy zapoznanie się z kodem źródłowym wszystkich aplikacji i, w razie potrzeby, s ręki do wszystkich dostawców plików ISV lub aplikacji. Pomoc techniczna firmy Microsoft może również dostarczyć listę aplikacji ADAL innych firm w Twojej dzierżawie.

**Migracja usługi AAD Graph**

W przypadku aplikacji korzystających z funkcji Azure AD Graph skorzystaj z naszych wskazówek dotyczących migrowania aplikacji usługi [Azure AD Graph do programu Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Nasz lista kontrolna dotycząca migracji stanowi punkt umożliwiający rozpoczęcie](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Portal rejestracji aplikacji Azure pokazuje, jakie aplikacje używają usługi AAD Graph. Zalecamy przejrzenie kodu źródłowego wszystkich Twoich aplikacji i, w razie potrzeby, skontaktowanie się z dowolnym dostawcą ISV lub dostawcą aplikacji. Pomoc techniczna firmy Microsoft może także udostępnić listę wszystkich użycia funkcji AAD Graph w dzierżawie.
3. Aby aplikacja uzyskać dostęp do danych w programie Microsoft Graph, użytkownik lub administrator musi udzielić odpowiednich uprawnień w ramach procesu wyrażania zgody. Odwołanie [do uprawnień programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) zawiera listę uprawnień skojarzonych z każdym głównym zestawem interfejsów API programu Microsoft Graph. Zawiera również wskazówki dotyczące korzystania z uprawnień.

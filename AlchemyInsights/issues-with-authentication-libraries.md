---
title: Problemy z bibliotekami uwierzytelniania
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063640"
---
# <a name="issues-with-authentication-libraries"></a>Problemy z bibliotekami uwierzytelniania

1. [Biblioteki uwierzytelniania platformy tożsamości firmy Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) zawiera listę obsługiwanych przez firmę Microsoft oraz zgodnych bibliotek klientów i oprogramowania pośredniczącego.
2. Biblioteka uwierzytelniania firmy Microsoft (MSAL) obsługuje kilka [przepływów uwierzytelniania](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) do użycia w różnych scenariuszach aplikacji.
3. Aby uwierzytelnić i uzyskać tokeny, należy zainicjować nową publiczną lub poufną aplikację kliencyjną w kodzie. Podczas inicjowania aplikacji klienckiej w bibliotece Microsoft Authentication Library (MSAL) możesz ustawić kilka opcji konfiguracji. Aby dowiedzieć się więcej, zobacz [opcje konfiguracji aplikacji.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Zakończenie świadczenia pomocy technicznej dla biblioteki ADAL (Azure Active Directory Authentication Library) i interfejsu API Azure AD Graph (AAD Graph)**

**Począwszy od 30 czerwca 2020 r.,** nie będziemy już dodawać żadnych nowych funkcji do funkcji ADAL i Azure AD Graph. Będziemy nadal zapewniać pomoc techniczną i aktualizacje zabezpieczeń, natomiast nie będziemy dłużej dostarczać aktualizacji funkcji.

**Począwszy od 30 czerwca 2022 r.,** zakończymy świadczenie pomocy technicznej dla funkcji ADAL i Azure AD Graph i nie będziemy już zapewniać pomocy technicznej ani aktualizacji zabezpieczeń.

Aplikacje korzystające z pliku ADAL w istniejących wersjach systemu operacyjnego będą nadal działać po tym czasie, ale nie będą otrzymać żadnych aktualizacji pomocy technicznej ani *zabezpieczeń.*

Aplikacje korzystające z funkcji Azure AD Graph po tym czasie mogą już nie otrzymywać odpowiedzi z punktu końcowego usługi Azure AD Graph.

**Migracja ADAL**

Zalecamy zaktualizowanie do [Biblioteki uwierzytelniania Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), która oferuje najnowsze aktualizacje funkcji i zabezpieczeń.

Jeśli korzystasz z aplikacji firmy Microsoft, wiesz, że firma Microsoft jest w trakcie migrowania jej aplikacji do programu MSAL do terminu zakończenia świadczenia pomocy technicznej, upewniając się, że odniesie korzyści z bieżących ulepszeń zabezpieczeń i funkcji pakietu MSAL.

Aby uzyskać więcej informacji, zobacz:

1. [Przeczytaj sekcję ADAL — często zadawane pytania](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Dowiedz się na temat sposobu migracji aplikacji zależnie od platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jeśli potrzebujesz pomocy w zrozumieniu, które z Twoich aplikacji korzystają z pliku ADAL, zalecamy przejrzenie kodu źródłowego wszystkich aplikacji, a w razie potrzeby słaniesz się z dowolnymi plikami ISV lub dostawcami aplikacji. Pomoc techniczna firmy Microsoft może również dostarczyć listę aplikacji ADAL innych firm w Twojej dzierżawie.

**Migracja usługi AAD Graph**

W przypadku aplikacji korzystających z funkcji Azure AD Graph skorzystaj z naszych wskazówek dotyczących migrowania aplikacji usługi [Azure AD Graph do programu Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Nasza lista kontrolna migracji stanowi punkt wyjścia.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Portal rejestracji aplikacji Azure pokazuje, jakie aplikacje używają usługi AAD Graph. Zalecamy przejrzenie kodu źródłowego wszystkich Twoich aplikacji i, w razie potrzeby, skontaktowanie się z dowolnym dostawcą ISV lub dostawcą aplikacji. Pomoc techniczna firmy Microsoft może także udostępnić listę wszystkich użycia funkcji AAD Graph w dzierżawie.
3. Aby aplikacja uzyskać dostęp do danych w programie Microsoft Graph, użytkownik lub administrator musi udzielić odpowiednich uprawnień w ramach procesu wyrażania zgody. Odwołanie [do uprawnień programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) zawiera listę uprawnień skojarzonych z każdym głównym zestawem interfejsów API programu Microsoft Graph. Zawiera również wskazówki dotyczące korzystania z uprawnień.

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
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028014"
---
# <a name="issues-with-authentication-libraries"></a>Problemy z bibliotekami uwierzytelniania

1. [Platforma tożsamości Microsoft uwierzytelniania zawiera](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) listę obsługiwanych przez firmę Microsoft oraz zgodnych bibliotek klientów i oprogramowania middleware.
2. Biblioteka uwierzytelniania firmy Microsoft (MSAL) obsługuje kilka przepływów [uwierzytelniania,](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) których można używać w różnych scenariuszach aplikacji.
3. Aby uwierzytelnić i uzyskać tokeny, inicjuje się nową publiczną lub poufną aplikację klienckią w kodzie. Podczas inicjowania aplikacji klienckiej w bibliotece Microsoft Authentication Library (MSAL) możesz ustawić kilka opcji konfiguracji. Aby dowiedzieć się więcej, zobacz [Opcje konfiguracji aplikacji.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Zakończenie świadczenia pomocy technicznej dla biblioteki ADAL (Azure Active Directory Authentication Library) i interfejsu API azure AD Graph (AAD Graph)**

**Począwszy od 30 czerwca 2020** r. nie będziemy już dodawać żadnych nowych funkcji do usługi ADAL ani Azure AD Graph. Będziemy nadal zapewniać pomoc techniczną i aktualizacje zabezpieczeń, natomiast nie będziemy dłużej dostarczać aktualizacji funkcji.

**Począwszy od 30 czerwca 2022 r.,** zakończymy świadczenie pomocy technicznej dla usługi ADAL i Azure AD Graph i nie będziemy już zapewniać pomocy technicznej ani aktualizacji zabezpieczeń.

Aplikacje korzystające z pliku ADAL w istniejących wersjach systemu operacyjnego będą nadal działać po tym czasie, ale nie będą korzystać z pomocy technicznej *ani aktualizacji zabezpieczeń.*

Aplikacje korzystające z usługi Azure AD Graph tym czasie mogą już nie odbierać odpowiedzi z punktu końcowego usługi Azure AD Graph sieci Web.

**Migracja ADAL**

Zalecamy zaktualizowanie do [Biblioteki uwierzytelniania Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), która oferuje najnowsze aktualizacje funkcji i zabezpieczeń.

Jeśli korzystasz z aplikacji firmy Microsoft, migruj aplikacje do programu MSAL do terminu zakończenia świadczenia pomocy technicznej, upewniając się, że będą one korzystać z bieżących ulepszeń zabezpieczeń i funkcji programu MSAL.

Więcej informacji można znaleźć w następujących artykułach:

1. [Przeczytaj sekcję ADAL — często zadawane pytania](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Dowiedz się na temat sposobu migracji aplikacji zależnie od platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jeśli potrzebujesz pomocy w zrozumieniu, które z Twoich aplikacji korzystają z pliku ADAL, zalecamy zapoznanie się ze wszystkimi kodami źródłowymi aplikacji i, jeśli to konieczne, spływaj do wszystkich usługodawców internetowych (ISV) lub dostawców aplikacji. Pomoc techniczna firmy Microsoft może również dostarczyć listę aplikacji ADAL innych firm w Twojej dzierżawie.

**Migracja usługi AAD Graph**

W przypadku aplikacji korzystających z usługi Azure AD Graph postępuj zgodnie z naszymi wskazówkami na temat migrowania aplikacji usługi [Azure AD Graph do usługi Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Nasza lista kontrolna migracji stanowi punkt wyjścia.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Portal rejestracji aplikacji Azure pokazuje, jakie aplikacje używają usługi AAD Graph. Zalecamy przejrzenie kodu źródłowego wszystkich Twoich aplikacji i, w razie potrzeby, skontaktowanie się z dowolnym dostawcą ISV lub dostawcą aplikacji. Pomoc techniczna firmy Microsoft może także udostępnić listę wszystkich funkcji AAD Graph użycia w Twojej dzierżawie.
3. Aby Twoja aplikacja uzyskać dostęp do danych w aplikacji Microsoft Graph, użytkownik lub administrator musi udzielić im właściwych uprawnień w ramach procesu zgody. Odwołanie [do Graph firmy Microsoft](https://docs.microsoft.com/graph/permissions-reference) zawiera listę uprawnień skojarzonych z każdym głównym zestawem interfejsów API usługi Microsoft Graph API. Zawiera również wskazówki dotyczące korzystania z tych uprawnień.

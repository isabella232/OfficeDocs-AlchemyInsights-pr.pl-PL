---
title: Problemy z tworzeniem aplikacji przy użyciu interfejsów API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975013"
---
# <a name="issues-developing-applications-with-apis"></a>Problemy z tworzeniem aplikacji przy użyciu interfejsów API

Aby rozpocząć korzystanie z interfejsu API Graph w usłudze Azure Active Directory, zobacz [Przewodnik Szybki Start dla interfejsu API Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) lub wyświetlanie [dokumentacji referencyjnej interfejsu API programu Azure AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Koniec obsługi biblioteki uwierzytelniania usługi Azure Active Directory (ADAL) i interfejsu API Azure AD Graph (usługa AAD Graph)**

**Od 30 czerwca 2020** r. nie będziemy już dodawać żadnych nowych funkcji do wykresu ADAL i Azure AD. Będziemy nadal dostarczać pomoc techniczną i aktualizacje zabezpieczeń, ale nie będą już udostępniać aktualizacji funkcji.

**Począwszy od 30 czerwca 2022** r., zostanie zakończona pomoc techniczna dla wykresu ADAL i Azure AD i nie będzie już udzielana pomoc techniczna ani aktualizacje zabezpieczeń.

Aplikacje używające biblioteki ADAL w istniejących wersjach systemu operacyjnego będą nadal działać po tym czasie, ale nie będą otrzymywać pomocy technicznej ani aktualizacji zabezpieczeń.

Aplikacje korzystające z programu Azure AD Graph już po upływie tego czasu nie możesz już odbierać odpowiedzi z punktu końcowego wykresu usługi Azure AD.

**Migracja biblioteki ADAL**

Zalecamy aktualizację do [biblioteki uwierzytelniania firmy Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), która ma najnowsze funkcje i aktualizacje zabezpieczeń.

Jeśli korzystasz z aplikacji firmy Microsoft, sprawdź, czy firma Microsoft jest w trakcie migrowania swoich aplikacji do MSAL przez ostateczny nieprzekraczalny termin, dzięki którym będą mogli korzystać z MSAL bieżących zabezpieczeń i funkcji.

1. [Przeczytaj często zadawane pytania dotyczące biblioteki ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Dowiedz się, jak przeprowadzić migrację aplikacji na poszczególnych platformach](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Jeśli potrzebujesz pomocy dotyczącej korzystania z aplikacji ADAL, zalecamy przejrzenie wszystkich kodów źródłowych aplikacji i w razie potrzeby skontaktowanie się z dostawcami ISV lub aplikacjami. Pomoc techniczna firmy Microsoft może również udostępnić listę wszystkich aplikacji innych niż Microsoft ADAL w dzierżawie.

**Migracja wykresu w usłudze AAD**

W przypadku aplikacji korzystających z usługi Azure AD Graph postępuj zgodnie z naszymi wskazówkami, aby przeprowadzić migrację [aplikacji Azure AD Graph do programu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Lista kontrolna migracji zawiera punkt wprowadzenia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Portal rejestracji aplikacji platformy Azure pokazuje, które aplikacje używają wykresu w usłudze AAD. Zalecamy przejrzenie wszystkich kodów źródłowych aplikacji, a w razie potrzeby skontaktowanie się z dostawcami ISV lub aplikacjami. Pomoc techniczna firmy Microsoft może również udostępnić listę wszystkich zastosowań wykresów w usłudze AAD w dzierżawie.
1. Aby aplikacja miała dostęp do danych w programie Microsoft Graph, użytkownik lub administrator musi udzielić mu odpowiednich uprawnień za pośrednictwem procesu wyrażania zgody. Informacje o uprawnieniach [programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) zawiera listę uprawnień skojarzonych z poszczególnymi zestawami interfejsów API programu Microsoft Graph. Zawiera również wskazówki dotyczące korzystania z tych uprawnień.

---
title: Praca z bibliotekami uwierzytelniania
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035825"
---
# <a name="working-with-authentication-libraries"></a>Praca z bibliotekami uwierzytelniania

Aby rozwiązać problem z biblioteką uwierzytelniania firmy Microsoft (MSAL), wykonaj następujące zalecane czynności:

1. **Praca z biblioteką MSAL:** [biblioteki uwierzytelniania platformy](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) tożsamości firmy Microsoft — w tym artykule przedstawiono obsługę biblioteki uwierzytelniania firmy Microsoft dla kilku typów aplikacji. Zawiera linki do kodu źródłowego biblioteki; gdzie uzyskać pakiet dla projektu aplikacji; oraz czy biblioteka obsługuje logowanie (uwierzytelnianie), dostęp do chronionych interfejsów API sieci Web (autoryzacji), czy oba te interfejsy.

2. **Rozwiązywanie problemów z** uwierzytelnianiem: Program MSAL obsługuje kilka przepływów uwierzytelniania, których można używać w różnych scenariuszach aplikacji. W zależności od sposobu, w jaki jest budowaną aplikację kliencową, msAL może używać co najmniej jednego przepływu uwierzytelniania obsługiwanego przez platformę tożsamości firmy Microsoft. Te przepływy mogą powodować tworzenie kilku typów tokenów i kodów autoryzacji oraz wymagać innych tokenów do ich działania.

3. **Tokeny dostępu:** [tokeny](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) dostępu platformy tożsamości firmy Microsoft — dowiedz się, jak interfejs API może weryfikować i używać roszczeń w tokenie dostępu. Cała dokumentacja w tym artykule, z wyjątkiem przypadków określonych, dotyczy tylko tokenów wystawionych dla zarejestrowanych interfejsów API. Nie mają one zastosowania do tokenów wystawionych dla interfejsów API należących do firmy Microsoft ani nie można ich używać do sprawdzania, jak platforma tożsamości firmy Microsoft będzie wystawiać tokeny dla tworzyć przez Ciebie interfejsu API.

**Zakończenie świadczenia pomocy technicznej dla biblioteki Azure Active Directory Authentication Library (ADAL)**

- **Począwszy od 30 czerwca 2020 r.,** nie będziemy już dodawać żadnych nowych funkcji do usługi ADAL i Azure AD Graph. Będziemy nadal zapewniać pomoc techniczną i aktualizacje zabezpieczeń, natomiast nie będziemy dłużej dostarczać aktualizacji funkcji.
- **Począwszy od 30 czerwca 2022 r.,** zakończymy świadczenie pomocy technicznej dla funkcji ADAL i Azure AD Graph i nie będziemy już zapewniać pomocy technicznej ani aktualizacji zabezpieczeń.
- Aplikacje korzystające z pliku ADAL w istniejących wersjach systemu operacyjnego będą nadal działać po tym czasie, ale nie będą korzystać z pomocy technicznej *ani aktualizacji zabezpieczeń.*
- Aplikacje używające funkcji Azure AD Graph po tym czasie mogą już nie otrzymywać odpowiedzi z punktu końcowego funkcji Azure AD Graph.

**Migracja ADAL**

- Zalecamy aktualizację do wersji MSAL, która zawiera najnowsze funkcje i aktualizacje zabezpieczeń.
- Jeśli korzystasz z aplikacji firmy Microsoft, migruj aplikacje do programu MSAL do terminu zakończenia świadczenia pomocy technicznej, upewniając się, że będą one korzystać z bieżących ulepszeń zabezpieczeń i funkcji programu MSAL.

1. [Przeczytaj często zadawane pytania dotyczące ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Dowiedz się, jak migrować aplikacje na platformie.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)
3. Jeśli po przeczytaniu przewodnika dla platformy aplikacji masz dodatkowe pytania, możesz opublikować wpis w usłudze [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) z tagiem [azure-ad-adal-deprecation] lub otworzyć problem w repozytorium GitHub biblioteki. Linki [do witryny](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) poszczególnych bibliotek można znaleźć w sekcji Języki i struktury w artykule z omówieniem funkcji **MSAL.**
4. **Jeśli potrzebujesz pomocy w zrozumieniu,** które z Twoich aplikacji używają pliku ADAL, zalecamy przejrzenie kodu źródłowego wszystkich aplikacji. W razie przypadku należy się z dostawcą oprogramowania (ISV) lub dostawcą aplikacji. Pomoc techniczna firmy Microsoft może również dostarczyć listę aplikacji ADAL innych firm w Twojej dzierżawie.








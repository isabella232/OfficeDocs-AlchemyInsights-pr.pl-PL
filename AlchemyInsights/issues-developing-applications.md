---
title: Problemy z tworzeniem aplikacji
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974772"
---
# <a name="issues-developing-applications"></a>Problemy z tworzeniem aplikacji

Aby rozwiązać najczęstsze problemy podczas budowania aplikacji usługi Azure Active Directory (AD), zobacz następujące artykuły:

- [Widzę problemy z logowaniem się do aplikacji tylko za pomocą przeglądarki Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Nie wiem, jak zmienić ustawienia domyślne okresu ważności tokenu dla mojej aplikacji](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Nie wiem, jak działa zgoda na stosowanie aplikacji](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Nie wiem, jak udzielić uprawnień do mojej aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nie rozumiem różnicy między uprawnieniami delegowanymi i aplikacjami](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Koniec obsługi biblioteki uwierzytelniania usługi Azure Active Directory (ADAL) i interfejsu API Azure AD Graph (usługa AAD Graph)** _

- Od 30 czerwca 2020 r. nie będziemy już dodawać żadnych nowych funkcji do biblioteki uwierzytelniania usługi Azure Active Directory (ADAL) i interfejsu API usługi Azure AD Graph (AAD Graph). Będziemy nadal dostarczać pomoc techniczną i aktualizacje zabezpieczeń, ale nie będą już udostępniać aktualizacji funkcji.

- Począwszy od 30 czerwca 2022 r., zostanie zakończona pomoc techniczna dla wykresu ADAL i AAD, dzięki czemu nie będzie już udzielana pomoc techniczna ani aktualizacje zabezpieczeń. W wyniku tego warunku obowiązują następujące implikacje:

    - Aplikacje używające biblioteki ADAL w istniejących wersjach systemu operacyjnego będą nadal działać po tym czasie, ale nie będą otrzymywać pomocy technicznej ani aktualizacji zabezpieczeń.

    - Aplikacje korzystające z wykresu AAD po upływie tego czasu mogą przestać otrzymywać odpowiedzi z punktu końcowego wykresu w usłudze AAD

*Migracja ADAL**

Jeśli korzystasz z aplikacji firmy Microsoft, Zalecamy zaktualizowanie biblioteki uwierzytelniania firmy Microsoft (MSAL), która ma najnowsze funkcje i aktualizacje zabezpieczeń. To zalecenie jest w kontekście firmy Microsoft inicjującej proces migrowania swoich aplikacji do MSAL przed upływem nieprzekraczalnego terminu na koniec obsługi. 

Migracja przez firmę Microsoft jej aplikacji na MSAL zapewnia, że aplikacje korzystają z bieżących udoskonaleń zabezpieczeń i funkcji usługi MSAL.

1. [Przeczytaj sekcję ADAL często zadawane pytania](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Dowiedz się, jak przeprowadzić migrację aplikacji na poszczególnych platformach](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Jeśli potrzebujesz pomocy w zrozumieniu, które aplikacje używają biblioteki ADAL, zalecamy przejrzenie wszystkich kodów źródłowych aplikacji i, jeśli to konieczne, dotarcie do wszystkich niezależnych dostawców oprogramowania (ISV) lub dostawców aplikacji. Pomoc techniczna firmy Microsoft może również udostępnić listę wszystkich aplikacji innych niż Microsoft ADAL w dzierżawie.

**Migracja wykresu w usłudze AAD**

W przypadku aplikacji korzystających z programu obsługi wykresów w usłudze AAD postępuj zgodnie z naszymi wskazówkami, aby przeprowadzić migrację aplikacji Graph

1. [Lista kontrolna migracji zawiera punkt wprowadzenia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Portal rejestracji aplikacji platformy Azure pokazuje, które aplikacje używają wykresu w usłudze AAD. Zalecamy przejrzenie wszystkich kodów źródłowych aplikacji i, jeśli to konieczne, do wszystkich niezależnych dostawców oprogramowania (ISV) lub dostawców aplikacji. Pomoc techniczna firmy Microsoft może także dostarczyć informacji na temat użycia wykresu w usłudze AAD w dzierżawie.








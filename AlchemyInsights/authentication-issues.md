---
title: Problemy z uwierzytelnianiem
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
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974796"
---
# <a name="authentication-issues"></a>Problemy z uwierzytelnianiem

**Szukasz informacji na temat kodów błędów AADSTS, które są zwracane z usługi Microsoft Azure Active Directory (STS)?** Zobacz [uwierzytelnianie w usłudze Azure AD kody błędów autoryzacji](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , aby znaleźć AADSTS błędów, poprawki i proponowane obejścia.

Błędy autoryzacji mogą być wynikiem kilku różnych problemów, z których większość generuje błąd 401 lub 403. Na przykład w przypadku błędów autoryzacji mogą wystąpić następujące problemy:

- Nieprawidłowe [przepływy pozyskiwania tokenów dostępu](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Źle skonfigurowane [zakresy uprawnień](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Brak [zgody](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Aby usunąć typowe błędy autoryzacji, spróbuj skorzystać z poniższych kroków, które najbardziej pasują do odbieranego błędu. W przypadku napotkanego błędu może wystąpić więcej niż jeden krok.

- **401 nieautoryzowany błąd: czy token jest prawidłowy?**

Upewnij się, że aplikacja przedstawia prawidłowy token dostępu do programu Microsoft Graph w ramach żądania. Ten błąd często oznacza, że token dostępu może być niedostępny w nagłówku żądania uwierzytelnienia HTTP lub że token jest nieprawidłowy lub wygasł. Stanowczo zalecamy użycie biblioteki uwierzytelniania firmy Microsoft (MSAL) do uzyskiwania dostępu do tokenów programu Access. Ponadto ten błąd może wystąpić, jeśli próbujesz użyć delegowanego tokenu dostępu przyznanego do osobistego konta Microsoft, aby uzyskać dostęp do interfejsu API obsługującego tylko konta służbowe (konta organizacji).

**403 zabroniony błąd: wybrano odpowiedni zestaw uprawnień?**

Upewnij się, że zażądano odpowiedniego zestawu uprawnień na podstawie interfejsów API programu Microsoft Graph, na które dzwonisz w aplikacji. Zalecane uprawnienia najmniej uprzywilejowane są dostępne we wszystkich tematach metod referencyjnych interfejsu API programu Microsoft Graph. Ponadto te uprawnienia muszą zostać przyznane aplikacji przez użytkownika lub administratora. Udzielanie uprawnień zwykle odbywa się za pośrednictwem strony zgody lub użycia bloku rejestracji aplikacji usługi Azure Portal. W bloku **Ustawienia** aplikacji kliknij pozycję **wymagane uprawnienia**, a następnie kliknij pozycję **Udziel uprawnień**. Aby uzyskać więcej informacji, zobacz:

- [Uprawnienia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Opis uprawnień usługi Azure AD i wyrażania zgody](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 zabroniony błąd: Czy Twoja aplikacja uzyskała token w celu dopasowania wybranych uprawnień?**

Upewnij się, że typy wymaganych uprawnień są zgodne z typem tokenu dostępu uzyskiwanym przez Twoją aplikację. Być może zażądasz i udzielasz uprawnień do aplikacji, ale używasz delegowanych tokenów przepływu kodu interaktywnego zamiast tokenów przepływu poświadczeń klienta lub żądam i udzielam uprawnień delegowanych, a nie tokenów przepływu kodu.

Aby uzyskać więcej informacji dotyczących nabywania tokenów, zobacz:

- [Uzyskiwanie dostępu w imieniu użytkowników i delegowanych uprawnień](https://docs.microsoft.com/graph/auth-v2-user) 
- [Przepływ kodu autoryzacji uwierzytelniania OAuth usługi Azure AD v 2.0 – 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Uzyskiwanie dostępu bez użytkownika (usługa demona) i uprawnienia aplikacji](https://docs.microsoft.com/graph/auth-v2-service) 
- [Przepływ poświadczeń klienta usługi Azure AD v 2.0-OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 zabroniony błąd: Resetowanie hasła**

Obecnie nie ma żadnych uprawnień usług "dostęp do usługi demon uprawnień aplikacji, które zezwalają na resetowanie haseł użytkowników. Te interfejsy API są obsługiwane tylko przy użyciu interaktywnego delegowanego kodu przepływu za pomocą zalogowanego administratora. Aby uzyskać więcej informacji, zobacz [uprawnienia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 zabroniony: czy użytkownik ma dostęp i jest licencjonowany?**

W przypadku delegowanych przepływów kodu program Microsoft Graph ocenia, czy żądanie zostało dozwolone na podstawie uprawnień przyznanych tej aplikacji oraz uprawnień, które posiada zalogowany użytkownik. Zazwyczaj ten błąd wskazuje, że użytkownik nie jest wystarczająco uprzywilejowany do wykonania żądania **lub** użytkownik nie ma licencji na dane, do których uzyskiwany jest dostęp. Żądanie może powiodło tylko użytkownicy z wymaganymi uprawnieniami lub licencjami.

**403 zabroniony: wybrano odpowiedni interfejs API zasobu?**

Usługi interfejsu API, takie jak Microsoft Graph, sprawdzają, czy roszczenie *AUD* (odbiorca) w otrzymanym tokenie dostępu jest zgodne z wartością oczekiwaną dla samej siebie, a jeśli nie, występuje błąd z niedozwolonym wystąpieniem 403. Typowy błąd powodujący błąd podczas próby użycia tokenu uzyskanego dla interfejsów API usługi Azure AD, interfejsów API programu Outlook lub interfejsów API programu SharePoint/OneDrive w celu nawiązania połączenia z programem Microsoft Graph (lub odwrotnie). Upewnij się, że zasób (lub zakres), w którym aplikacja otrzymuje token, odpowiada interfejsowi API, do którego aplikacja jest wywoływana.

**400 złe żądanie lub 403 zabronione: czy użytkownik jest zgodny z zasadami obowiązującymi w organizacji dostępu warunkowego (UC)?**

Na podstawie zasad obowiązujących w organizacji (UC) użytkownik może zabrać dostęp do zasobów programu Microsoft Graph za pośrednictwem aplikacji, aby uzyskać dodatkowe informacje, których nie ma w tokenie dostępu pierwotnie uzyskanej przez aplikację. W tym przypadku aplikacja otrzymuje **400 z błędem *interaction_required*** podczas pobierania tokenu dostępu lub 403 z błędem ***insufficient_claims*** podczas wywoływania programu Microsoft Graph. W obu przypadkach odpowiedź na błąd zawiera dodatkowe informacje, które mogą być przedstawiane autoryzowanemu punktowi końcowemu w celu zakwestionowania użytkownika w celu uzyskania dodatkowych informacji (takich jak uwierzytelnianie wieloskładnikowe lub rejestracja urządzeń).

Aby uzyskać więcej informacji dotyczących dostępu warunkowego, zobacz:

- [Obsługiwanie wyzwań dotyczących dostępu warunkowego przy użyciu MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Wskazówki dla programistów dotyczące dostępu warunkowego usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Koniec obsługi biblioteki uwierzytelniania usługi Azure Active Directory (ADAL) i interfejsu API Azure AD Graph (usługa AAD Graph)_* _

- Od 30 czerwca 2020 r. nie będziemy już dodawać żadnych nowych funkcji do biblioteki uwierzytelniania usługi Azure Active Directory (ADAL) i interfejsu API usługi Azure AD Graph (AAD Graph). Będziemy nadal dostarczać pomoc techniczną i aktualizacje zabezpieczeń, ale nie będą już udostępniać aktualizacji funkcji.
- Począwszy od 30 czerwca 2022 r., zostanie zakończona pomoc techniczna dla wykresu ADAL i AAD, dzięki czemu nie będzie już udzielana pomoc techniczna ani aktualizacje zabezpieczeń.
    - Aplikacje używające biblioteki ADAL w istniejących wersjach systemu operacyjnego będą nadal działać po tym czasie, ale nie będą otrzymywać pomocy technicznej ani aktualizacji zabezpieczeń.
    - Aplikacje korzystające z wykresu w usłudze AAD po upływie tego czasu mogą przestać odbierać odpowiedzi z punktu końcowego wykresu w usłudze AAD.

*Migracja ADAL**

Zalecamy aktualizację do [biblioteki uwierzytelniania firmy Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), która ma najnowsze funkcje i aktualizacje zabezpieczeń. To zalecenie dotyczy firmy Microsoft migrowania swoich aplikacji do MSAL przez nieprzekraczalny termin końca obsługi. Celem migracji aplikacji firmy Microsoft do MSAL jest zapewnienie, że aplikacje będą korzystały z bieżących ulepszeń zabezpieczeń i funkcji MSAL.

- [Przeczytaj sekcję ADAL często zadawane pytania](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Dowiedz się, jak przeprowadzić migrację aplikacji na poszczególnych platformach](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Jeśli potrzebujesz pomocy dotyczącej korzystania z aplikacji ADAL, zalecamy przejrzenie wszystkich kodów źródłowych aplikacji i w razie potrzeby skontaktowanie się z niektórymi dostawcami oprogramowania (ISV) lub dostawcami aplikacji. Pomoc techniczna firmy Microsoft może również udostępnić listę wszystkich aplikacji innych niż Microsoft ADAL w dzierżawie.

**Migracja wykresu w usłudze AAD**

W przypadku aplikacji korzystających z funkcji Graph na platformie AAD postępuj zgodnie z naszymi wskazówkami, aby [przeprowadzić migrację aplikacji Azure AD Graph do programu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Lista kontrolna migracji zawiera punkt wprowadzenia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Portal rejestracji aplikacji platformy Azure pokazuje, które aplikacje używają wykresu w usłudze AAD. Zalecamy przejrzenie wszystkich kodów źródłowych aplikacji, a w razie potrzeby skontaktowanie się z dostawcami ISV lub aplikacjami. Pomoc techniczna firmy Microsoft może także dostarczyć informacje dotyczące całego użycia wykresu w usłudze AAD w dzierżawie.

 











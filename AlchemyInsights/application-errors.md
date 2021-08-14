---
title: Błędy aplikacji
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
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931459"
---
# <a name="application-errors"></a>Błędy aplikacji

Szukasz informacji na temat kodów błędów **AADSTS** zwracanych z usługi tokenu zabezpieczeń usługi Azure Active Directory (Azure AD)? Przeczytaj [kody błędów uwierzytelniania i autoryzacji](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) usługi Azure AD, aby znaleźć opisy błędów usługi AADSTS, poprawki i niektóre sugerowane obejścia.

Błędy uwierzytelniania mogą wynikać z wielu różnych problemów, z czego większość z nich generuje błąd 401 lub 403. Na przykład do błędów autoryzacji mogą prowadzić następujące elementy:

- Nieprawidłowe [przepływy uzyskiwania tokenu dostępu](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes), 
- Źle skonfigurowane [zakresy uprawnień](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes), 
- Brak [zgody](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent).

Aby rozwiązać typowe błędy autoryzacji, spróbuj wykonać podane poniżej czynności, które są najbardziej zbliżone do zwracanych błędów. Może mieć zastosowanie więcej niż jeden.

**Nieautoryzowany błąd 401: Czy Twój token jest prawidłowy?**

Upewnij się, że w ramach żądania Twoja aplikacja prezentuje prawidłowy token dostępu Graph do firmy Microsoft. Ten błąd często oznacza, że w nagłówku żądania uwierzytelniania HTTP może brakować token dostępu, lub token jest nieprawidłowy bądź upłynęła jego ważność. Zdecydowanie zalecamy uzyskanie dostępu do tokenu za pomocą biblioteki [Microsoft Authentication Library (MSAL).](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) Ponadto ten błąd może wystąpić w przypadku próby użycia tokenu dostępu delegowanego przyznanego na osobistym koncie Microsoft w celu uzyskania dostępu do interfejsu API obsługującego tylko konta służbowe (konta organizacji).

**Błąd zabroniony 403: Czy wybrano prawidłowy zestaw uprawnień?**

Upewnij się, że zażądano poprawnego zestawu uprawnień na podstawie interfejsów API usługi Microsoft Graph Twoich połączeń aplikacji. Zalecane uprawnienia o najmniejszych uprawnieniach podano we wszystkich tematach dotyczących metod Graph API firmy Microsoft. Ponadto uprawnienia te muszą być przyznane aplikacji przez użytkownika lub administratora. Udzielanie uprawnień zwykle odbywa się za pośrednictwem strony zgody lub przez udzielenie uprawnień przy użyciu narzędzia do rejestracji aplikacji Azure Portal. Z poziomu bloku **Ustawienia** dla danej aplikacji kliknij pozycję **Wymagane uprawnienia**, a następnie kliknij pozycję **Udzielanie uprawnień**.

- [Uprawnienia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Opis uprawnień i zgody w usłudze Microsoft Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Błąd zabroniony 403: Czy Twoja aplikacja pozyskała token zgodny z wybranymi uprawnieniami?**

Upewnij się, że typ żądanych lub przyznanych uprawnień jest taki, jak typ tokenu dostępu nabytego przez aplikację. Być może żądasz i udzielasz uprawnień aplikacji, ale używasz tokenów delegowanego przepływu interakcyjnego kodu zamiast tokenów przepływu poświadczeń klienta albo żądasz i udzielasz uprawnień delegowanych, ale używasz tokenów przepływu poświadczeń klienta zamiast tokenów przepływu delegowanego kodu.

- [Uzyskiwanie dostępu w imieniu użytkowników oraz delegowane uprawnienia](https://docs.microsoft.com/graph/auth_v2_user) 
- [Microsoft Azure Active Directory wer. 2.0 — przepływ kodu autoryzacji OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Uzyskiwanie dostępu bez uprawnień użytkownika (usługi demona) i aplikacji](https://docs.microsoft.com/graph/auth_v2_service) 
- [Microsoft Azure Active Directory wer. 2.0 — przepływ poświadczeń klienta OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Błąd zabroniony 403: resetowanie haseł**

Obecnie nie istnieją uprawnienia usługi demon dla uprawnień aplikacji między usługami, które umożliwiają resetowanie haseł użytkowników. Te interfejsy API są obsługiwane wyłącznie przy użyciu przepływów interakcyjnych delegowanych kodów z zalogowanym administratorem.

- [Uprawnienia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**Zabroniony 403: Czy użytkownik ma dostęp i jest on licencjonowany?**

W przypadku przepływów kodu delegowanego usługa Microsoft Graph ocenia, czy żądanie jest dozwolone na podstawie uprawnień przyznanych aplikacji i uprawnień, które ma zalogowany użytkownik. Błąd ten zazwyczaj wskazuje, że użytkownik nie jest wystarczającego uprawniony do wykonania żądania  lub użytkownik nie jest licencjonowany w zakresie danych, do których uzyskuje dostęp. Tylko użytkownicy z wymaganymi uprawnieniami lub licencjami mogą pomyślnie wykonać żądanie.

**Zabroniony 403: Czy wybrano poprawny interfejs API zasobu?**

Usługi interfejsu API, takie jak Microsoft Graph, sprawdzają, czy żądanie usd (grupa odbiorców) w otrzymanym tokenie dostępu jest takie same, jak oczekiwana przez niego wartość, a jeśli nie jest, powoduje błąd 403 dostęp zabroniony. Typową pomyłką powodującą wystąpienie tego błędu jest próba używania tokenu pozyskanego dla interfejsów API usługi Azure AD Graph, interfejsów API programu Outlook lub interfejsów API SharePoint/OneDrive do wywołania programu Microsoft Graph (lub na odwrót). Upewnij się, że zasób (lub zakres), dla którego Twoja aplikacja pozyskuje token, odpowiada interfejsowi API, który aplikacja wywołuje.

**Nieprawidłowe żądanie 400 lub Zabroniony 403: Czy użytkownik spełnia zasady dostępu warunkowego (CA) swojej organizacji?**

Zgodnie z zasadami certyfikacji organizacji użytkownik, który uzyskuje dostęp do zasobów usługi Microsoft Graph za pośrednictwem Twojej aplikacji, może być poddany wyzwaniu w celu uzyskania dodatkowych informacji, które nie są dostępne w tokenie dostępu, który nabył Twoja aplikacja. W takim przypadku Twoja aplikacja otrzyma 400 z błędem *interaction_required* podczas pozyskiwania tokenu dostępu bądź 403 z błędem *insufficient_claims* w przypadku wywoływania programu Microsoft Graph. W obu przypadkach odpowiedź na błąd zawiera dodatkowe informacje, które można zaprezentować dla punktu końcowego autoryzowania w celu zasypowania użytkownika dodatkowymi informacjami (na przykład uwierzytelnianie wieloskładnikowe lub rejestracja urządzenia).

- [Obsługa problemów z dostępem warunkowym przy użyciu programu MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Wskazówki dla deweloperów w zakresie dostępu warunkowego usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)

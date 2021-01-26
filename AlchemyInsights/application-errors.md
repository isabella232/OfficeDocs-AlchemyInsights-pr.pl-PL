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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984583"
---
# <a name="application-errors"></a>Błędy aplikacji

Szukasz informacji na temat **kodów błędów AADSTS** , które są zwracane z usługi Microsoft Azure Active Directory (STS)? Zapoznaj się z [kodami błędów uwierzytelniania i autoryzacji usługi Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , aby znaleźć AADSTS błędów, poprawki i proponowane obejścia.

Błędy autoryzacji mogą być wynikiem kilku różnych problemów, z których większość generuje błąd 401 lub 403. Na przykład w przypadku problemów z autoryzacją mogą wystąpić następujące błędy:

- Nieprawidłowe [przepływy pozyskiwania tokenów dostępu](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Źle skonfigurowane [zakresy uprawnień](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Brak [zgody](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Aby usunąć typowe błędy autoryzacji, spróbuj wykonać poniższe czynności, które najbardziej pasują do odbieranego błędu. Może obowiązywać więcej niż jedna z nich.

**401 nieautoryzowany błąd: czy token jest prawidłowy?**

Upewnij się, że aplikacja przedstawia prawidłowy token dostępu do programu Microsoft Graph w ramach żądania. Ten błąd często oznacza, że token dostępu może być niedostępny w nagłówku żądania uwierzytelnienia HTTP lub że token jest nieprawidłowy lub wygasł. Stanowczo zalecamy użycie [biblioteki uwierzytelniania firmy Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) do uzyskiwania dostępu do tokenów programu Access. Ponadto ten błąd może wystąpić, jeśli próbujesz użyć delegowanego tokenu dostępu przyznanego do osobistego konta Microsoft, aby uzyskać dostęp do interfejsu API obsługującego tylko konta służbowe (konta organizacji).

**403 zabroniony błąd: wybrano odpowiedni zestaw uprawnień?**

Upewnij się, że zażądano odpowiedniego zestawu uprawnień na podstawie interfejsów API programu Microsoft Graph, na które dzwonisz. Zalecane najmniej uprzywilejowane uprawnienia są dostępne we wszystkich tematach metod referencyjnych interfejsu API programu Microsoft Graph. Ponadto te uprawnienia muszą zostać przyznane aplikacji przez użytkownika lub administratora. Udzielanie uprawnień zwykle odbywa się za pośrednictwem strony zgody lub udzielania uprawnień przy użyciu bloku rejestracji aplikacji Azure Portal. W bloku **Ustawienia** aplikacji kliknij pozycję **wymagane uprawnienia**, a następnie kliknij pozycję **Udziel uprawnień**.

- [Uprawnienia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Opis uprawnień usługi Azure AD i wyrażania zgody](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 zabroniony błąd: Czy Twoja aplikacja uzyskała token w celu dopasowania wybranych uprawnień?**

Upewnij się, że typ uprawnień żądany lub udzielony jest zgodny z typem tokenu dostępu pobieranego przez Twoją aplikację. Być może zażądasz i udzielasz uprawnień do aplikacji, ale używasz delegowanych tokenów przepływu kodu interaktywnego zamiast tokenów przepływu poświadczeń klienta lub żądam i udzielam uprawnień delegowanych, a nie tokenów przepływu kodu.

- [Uzyskiwanie dostępu w imieniu użytkowników i delegowanych uprawnień](https://docs.microsoft.com/graph/auth_v2_user) 
- [Przepływ kodu autoryzacji uwierzytelniania OAuth usługi Azure AD v 2.0 – 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Uzyskiwanie dostępu bez użytkownika (usługa demona) i uprawnienia aplikacji](https://docs.microsoft.com/graph/auth_v2_service) 
- [Przepływ poświadczeń klienta usługi Azure AD v 2.0-OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 zabroniony błąd: Resetowanie hasła**

Obecnie nie ma żadnych uprawnień usług "dostęp do usługi demon uprawnień aplikacji, które zezwalają na resetowanie haseł użytkowników. Te interfejsy API są obsługiwane tylko przy użyciu interaktywnego delegowanego kodu przepływu za pomocą zalogowanego administratora.

- [Uprawnienia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 zabroniony: czy użytkownik ma dostęp i jest licencjonowany?**

W przypadku delegowanych przepływów kodu program Microsoft Graph ocenia, czy żądanie jest dozwolone na podstawie uprawnień przyznanych tej aplikacji oraz uprawnień, które posiada zalogowany użytkownik. Zazwyczaj ten błąd wskazuje, że użytkownik nie jest wystarczająco uprzywilejowany do wykonania żądania lub użytkownik nie ma licencji na dane, do których uzyskiwany jest dostęp. Żądanie może powiodło tylko użytkownicy z wymaganymi uprawnieniami lub licencjami.

**403 zabroniony: wybrano odpowiedni interfejs API zasobu?**

Usługi interfejsu API, takie jak Microsoft Graph, sprawdzają, czy Auda (odbiorca) w otrzymanym tokenie dostępu jest zgodna z oczekiwaną wartością, a jeśli nie, powoduje błąd zabroniony 403. Typowy błąd powodujący błąd podczas próby użycia tokenu uzyskanego dla interfejsów API usługi Azure AD, interfejsów API programu Outlook lub interfejsów API programu SharePoint/OneDrive w celu nawiązania połączenia z programem Microsoft Graph (lub odwrotnie). Upewnij się, że zasób (lub zakres), w którym aplikacja otrzymuje token, odpowiada interfejsowi API, do którego aplikacja jest wywoływana.

**400 złe żądanie lub 403 zabronione: czy użytkownik jest zgodny z zasadami obowiązującymi w organizacji dostępu warunkowego (UC)?**

Na podstawie zasad urzędu certyfikacji organizacji użytkownik może zabrać dostęp do zasobów programu Microsoft Graph za pośrednictwem aplikacji, aby uzyskać dodatkowe informacje, których nie ma w tokenie dostępu pierwotnie uzyskanego przez aplikację. W tym przypadku aplikacja otrzymuje 400 z błędem *interaction_required* podczas pobierania tokenu dostępu lub 403 z błędem *Insufficient_claims* podczas wywoływania programu Microsoft Graph. W obu przypadkach odpowiedź na błąd zawiera dodatkowe informacje, które mogą być prezentowane w celu autoryzowania punktu końcowego, aby zakwestionować użytkownika pod kątem dodatkowych informacji (takich jak uwierzytelnianie wieloskładnikowe lub rejestracja urządzeń).

- [Obsługiwanie wyzwań dotyczących dostępu warunkowego przy użyciu MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Wskazówki dla programistów dotyczące dostępu warunkowego usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)

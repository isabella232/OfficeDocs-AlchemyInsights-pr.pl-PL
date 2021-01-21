---
title: Problemy z tokenami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917038"
---
# <a name="issues-with-tokens"></a>Problemy z tokenami

Aby zarządzać problemami związanymi z tokenami, można wykonać następujące czynności:

1. Możesz określić okres istnienia, jaki ma mieć dostęp, identyfikator lub token SAML wystawiony przez platformę Microsoft Identity. Możesz ustawić okresy ważności tokenów dla wszystkich aplikacji w organizacji, dla aplikacji z wieloma dzierżawami (wielu organizacji) lub dla określonego podmiotu zabezpieczeń usługi w organizacji. Aby uzyskać więcej informacji, zobacz [konfigurowalne okresy ważności tokenów w usłudze Microsoft Identity platform (wersja Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Tokeny dostępu umożliwiają klientom bezpieczne nawiązywanie połączeń za pomocą interfejsów API sieci Web oraz uwierzytelnianie i autoryzację przy użyciu interfejsów API sieci Web. Zgodnie z specyfikacją OAuth tokeny dostępu są nieprzezroczystymi ciągami bez zestawu, a u innych dostawców tożsamości (IDPs) używają identyfikatorów GUID, inne używają zaszyfrowanych obiektów BLOB. Platforma tożsamości firmy Microsoft korzysta z różnych formatów tokenów dostępu, w zależności od konfiguracji interfejsu API, który akceptuje token. Aby dowiedzieć się, jak interfejs API może sprawdzać i stosować oświadczenia w tokenie dostępu, zobacz [tokeny dostępu platformy Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Biblioteka uwierzytelniania firmy Microsoft (MSAL) obsługuje kilka przepływów uwierzytelniania, które można wykorzystać w różnych scenariuszach aplikacji. Aby uzyskać więcej informacji, zobacz [przepływy uwierzytelniania](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Za pomocą kodu autoryzacji OAuth 2,0 można korzystać w aplikacjach zainstalowanych na urządzeniu w celu uzyskania dostępu do chronionych zasobów, takich jak internetowe interfejsy API. Korzystając z implementacji platformy Microsoft Identity platform uwierzytelniania OAuth 2,0, możesz dodać funkcję logowania i korzystania z interfejsu API do aplikacji mobilnych i klasycznych. Zobacz [przepływ kodu autoryzacji Microsoft Identity platform i OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) , aby korzystać bezpośrednio z protokołu w aplikacji, korzystając z dowolnego języka.
5. OpenID Connect (OIDC) jest protokołem uwierzytelniania opartym na 2,0 OAuth, za pomocą którego można bezpiecznie zalogować użytkownika do aplikacji. Gdy korzystasz z implementacji programu OpenID Connect w punkcie końcowym Microsoft Identity platform, możesz dodać do aplikacji uprawnienia do logowania i korzystania z interfejsu API. W [protokole Microsoft Identity platform i OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) jest wyświetlana Metoda niezależna od języka oraz opis sposobu wysyłania i odbierania wiadomości HTTP bez użycia bibliotek Microsoft Open Source.
    - Punkt końcowy UserInfo jest częścią standardu OIDC, który umożliwia zwracanie oświadczeń dotyczących użytkownika, który został uwierzytelniony. Aby uzyskać więcej informacji, zobacz [punkt końcowy informacji o firmie Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - [Wywołanie internetowego interfejsu API w aplikacji sieci Web przy użyciu przykładu usługi Azure AD i OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) przykładowe pokazuje, jak utworzyć aplikację sieci Web MVC korzystającą z usługi Azure AD do logowania przy użyciu protokołu OpenID Connect, a następnie zadzwonić do internetowego interfejsu API pod tożsamością zalogowanego użytkownika przy użyciu tokenów uzyskanych za pośrednictwem uwierzytelniania OAuth 2,0. W tym przykładzie użyto oprogramowania OpenID Connect ASP .NET OWIN i ADAL .NET.
6. [Skonfiguruj aplikację w celu udostępnienia internetowego interfejsu API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -w tym szybkim połączeniu możesz zarejestrować internetowy interfejs API za pomocą platformy tożsamości Microsoft i uwidocznić go aplikacjom klienckim, dodając przykładowy zakres. Rejestrując interfejs API sieci Web i uwidaczniając go za pośrednictwem zakresów, można udostępnić swoim zasobom dostęp do zasobów autoryzowanym użytkownikom i aplikacjom klienckim, które uzyskają dostęp do interfejsu API.
7. W usłudze Azure Active Directory B2C (Azure AD B2C) przepływ poświadczeń hasła właściciela zasobów (ROPC) jest przepływem standardowego uwierzytelniania OAuth. W tym przepływie aplikacja, nazywana również jednostką uzależnioną, wymienia prawidłowe poświadczenia dla tokenów. Poświadczenia zawierają identyfikator użytkownika i hasło. Zwrócone tokeny to token identyfikatora, token dostępu i token odświeżania. Aby uzyskać więcej informacji, zobacz [Konfigurowanie przepływu poświadczeń hasła właściciela zasobów w usłudze Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 


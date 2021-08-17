---
title: Rozwiązywanie problemów z bezproblemowym logowaniem jednokrotnym opartym na centrum OIDC
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105788"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Rozwiązywanie problemów z bezproblemowym logowaniem jednokrotnym opartym na centrum OIDC

- Aby dowiedzieć się, jak dodać aplikację opartą na usłudze OIDC do dzierżawy platformy Azure, zobacz Szybki start: konfigurowanie logowania jednokrotnego opartego na usłudze OIDC dla aplikacji w dzierżawie usługi [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Aby uzyskać więcej szczegółowych informacji na temat aplikacji, które korzystają ze standardu OpenID Połączenie do wdrażania logowania pojedynczego, zobacz Opis logowania pojedynczego opartego na standardzie [OIDC.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Aby uzyskać informacje na wypadek, gdy wybierzesz pisanie kodu, wysyłając bezpośrednio żądania HTTP i obsługuj je lub używając biblioteki open source innej firmy, a nie za pomocą jednej z naszych bibliotek open source, zobacz protokoły [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)i OpenID Połączenie w sieci Platforma tożsamości Microsoft.

**Protokoły**

1. [Platforma tożsamości Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) i niejawny przepływ przyznawania — definiujący typ przyznawania niejawnego jest taki, że tokeny (tokeny identyfikatorów lub tokeny dostępu) są zwracane bezpośrednio z punktu końcowego /authorize zamiast punktu końcowego /token. Jest to często używane jako część przepływu kodu autoryzacji w tak zwanym "przepływie hybrydowym" — pobierania tokenu identyfikatora dla żądania /authorize wraz z kodem **autoryzacji.** W tym artykule opisano, jak programować bezpośrednio za pomocą protokołu w aplikacji w celu żądania tokenów z usługi Azure AD.
2. Platforma tożsamości Microsoft i Przepływ kodu autoryzacji [protokołu OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) — grant kodu autoryzacji OAuth 2.0 może być używany w aplikacjach zainstalowanych na urządzeniu w celu uzyskania dostępu do chronionych zasobów, takich jak interfejsy API sieci Web. Za pomocą Platforma tożsamości Microsoft OAuth 2.0 możesz dodać dostęp logowania i interfejsu API do aplikacji **mobilnych i klasycznych.** W tym artykule opisano, jak programować bezpośrednio za pomocą protokołu w aplikacji w dowolnym języku.
3. Platforma tożsamości Microsoft i [OpenID Połączenie —](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) podczas korzystania z implementacji usługi OpenID Połączenie przez Platforma tożsamości Microsoft można dodać do aplikacji dostęp logowania i interfejsu API. W tym artykule pokazano, jak to zrobić niezależnie od języka i opisano sposób wysyłania i odbierania wiadomości HTTP bez korzystania z jakichkolwiek bibliotek **open source firmy Microsoft.**
4. Platforma tożsamości Microsoft i przepływ poświadczeń klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) — aby uzyskać dostęp do zasobów hostowanych w sieci Web przy użyciu tożsamości aplikacji, można użyć grantu poświadczeń klienta OAuth 2.0 określonego w dokumencie RFC 6749, czasami nazywanym dwuedytowanymi poświadczeniami **OAuth.** Tego typu udzielanie jest często używane w przypadku interakcji między serwerami, które muszą być uruchamiane w tle, bez bezpośredniej interakcji z użytkownikiem. Te typy aplikacji są często nazywane **daemonami** lub **kontami usług.** W tym artykule opisano, jak programować bezpośrednio na podstawie protokołu w aplikacji.

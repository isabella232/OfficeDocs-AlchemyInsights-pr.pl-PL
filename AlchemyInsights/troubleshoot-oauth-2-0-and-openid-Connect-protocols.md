---
title: Rozwiązywanie problemów z protokołami OAuth 2.0 i OpenID Connect
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
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037692"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Rozwiązywanie problemów z protokołami OAuth 2.0 i OpenID Connect

Aby rozwiązać problemy z protokołu OAuth 2.0 i OpenID Connect, wykonaj następujące zalecane czynności:

Zapoznaj się z następującymi artykułami związanymi z konfiguracją i rozwiązywaniem problemów z protokołami OAuth 2.0 i OpenID Connect:

- Platforma tożsamości firmy Microsoft i przepływ kodu autoryzacji [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) — w tym artykule opisano, jak programować bezpośrednio przy użyciu przepływu przyznawania kodu **(PKCE)** w aplikacji, używając dowolnego języka.
- Platforma tożsamości firmy Microsoft i przepływ poświadczeń klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) — w tym artykule opisano, jak programować bezpośrednio z przepływem poświadczeń klienta **w** aplikacji.
- Platforma tożsamości firmy Microsoft i poświadczenia hasła właściciela zasobu [2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) — w tym artykule opisano, jak programować bezpośrednio w aplikacji przy użyciu przepływu **DOC.**
    - Platforma tożsamości firmy Microsoft obsługuje tylko program PROCD dla dzierżaw usługi Azure AD, a nie dla kont osobistych. Oznacza to, że należy użyć punktu końcowego **dzierżawy (lub https://login.microsoftonline.com/{TenantId_or_Name})** punktu **końcowego organizacji).**
    - Konta osobiste zaproszone do dzierżawy usługi Azure AD nie mogą korzystać z funkcjiKIC.
    - Konta bez haseł nie mogą logować się za pośrednictwem tego systemu. W tym scenariuszu zalecamy używanie innego przepływu dla aplikacji.
    - Użytkownicy, którzy będą logować się do aplikacji przy użyciu uwierzytelniania wieloskładnikowego [(MFA, multi-factor authentication),](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) zostaną zablokowani.
    - PROGRAM DOC nie jest obsługiwany [w](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) scenariuszach federacji tożsamości hybrydowej (na przykład w usługach Azure AD i ADFS używanych do uwierzytelniania kont lokalnych). Jeśli użytkownicy są przekierowani na pełną stronę do lokalnego dostawcy tożsamości, usługa Azure AD nie może przetestować nazwy użytkownika i hasła względem tego dostawcy tożsamości. [Uwierzytelnianie pass-through](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) jest jednak obsługiwane przez kodER-TOC.
    - Wyjątek do scenariusza federacji tożsamości hybrydowej może być następujący: Zasady odnajdowania realm głównego z ustawieniem **AllowCloudPasswordValidation** ustawionym na wartość **TRUE** umożliwią pracę przepływu PRACC dla użytkowników federowanych, gdy hasło lokalne jest synchronizowane z chmurą. Aby uzyskać więcej informacji, zobacz Włączanie bezpośredniego uwierzytelniania [OKC użytkowników federowanych dla starszych aplikacji.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- Platforma tożsamości firmy Microsoft i przepływ [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) w imieniu — w tym artykule opisano, jak programować bezpośrednio przepływ w **imieniu użytkownika (OBO)** w aplikacji.
- [Platforma tożsamości firmy Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) i protokół OpenID Connect — w tym artykule pokazano, jak wdrożyć protokół OpenID Connect niezależnie od języka, a także opisano sposób wysyłania i odbierania wiadomości HTTP bez korzystania z jakichkolwiek bibliotek open source firmy Microsoft.

**Tokeny dostępu**

[Tokeny dostępu platformy](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) tożsamości firmy Microsoft — dowiedz się, jak interfejs API może sprawdzać poprawność roszczeń wewnątrz tokenu dostępu i korzystać z nich. Cała dokumentacja w tym artykule, z wyjątkiem przypadków określonych, dotyczy tylko tokenów wystawionych dla zarejestrowanych interfejsów API. Nie mają one zastosowania do tokenów wystawionych dla interfejsów API należących do firmy Microsoft ani nie można ich używać do sprawdzania, jak platforma tożsamości firmy Microsoft będzie wystawiać tokeny dla tworzyć przez Ciebie interfejsu API.

**Konfiguracja aplikacji**

[Ograniczenia i limity](https://docs.microsoft.com/azure/active-directory/develop/reply-url) dotyczące przekierowania URI (adresu URL odpowiedzi) — dowiedz się, jak skonfigurować adres URL przekierowania (adresu URL odpowiedzi). Identyfikator URI przekierowania (adres URL odpowiedzi) to lokalizacja, w której serwer autoryzacji wysyła do użytkownika po pomyślnym dokonaniu autoryzacji i przyznaniu kodu autoryzacji lub tokenu dostępu. Serwer autoryzacji wysyła kod lub token do URI przekierowywania. dlatego ważne jest, aby zarejestrować prawidłową lokalizację w ramach procesu rejestracji aplikacji.

**Inicjowanie obsługi administracyjnej aplikacji**

[Samouczek: opracowywanie i planowanie](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) inicjowania obsługi administracyjnej dla punktu końcowego programu SCIM — w tym artykule opisano, jak utworzyć punkt końcowy programu SCIM i zintegrować go z usługą inicjowania obsługi administracyjnej AAD.



---
title: Problemy z uwierzytelnianiem
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
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976859"
---
# <a name="authentication-issues"></a>Problemy z uwierzytelnianiem

**Szukasz informacji o kodach błędów AADSTS, które są zwracane z usługi tokenu zabezpieczającego (STS) Azure Active Directory (Azure AD)?** Zobacz [Uwierzytelnianie Microsoft Azure Active Directory i kody błędów uwierzytelniania](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes), aby uzyskać opisy błędów AADSTS, poprawki i niektóre sugerowane obejścia.

Błędy uwierzytelniania mogą wynikać z wielu różnych problemów, z czego większość z nich generuje błąd 401 lub 403. Poniższe problemy mogą na przykład doprowadzać do wystąpienia błędów:

- Nieprawidłowe [przepływy uzyskiwania tokenu dostępu](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization), 
- Źle skonfigurowane [zakresy uprawnień](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent), 
- Brak [zgody](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent).

Aby rozwiązać typowe błędy uwierzytelniania, spróbuj wykonać kroki opisane poniżej, które najlepiej są dopasowane do otrzymywanego błędu. W przypadku otrzymywanego błędu można zastosować więcej niż jeden krok.

**Nieautoryzowany błąd 401: Czy Twój token jest prawidłowy?**

Upewnij się, że Twoja aplikacja zgłasza w programie Microsoft Graph prawidłowy token dostępu jako część żądania. Ten błąd często oznacza, że w nagłówku żądania uwierzytelniania HTTP może brakować token dostępu, lub token jest nieprawidłowy bądź upłynęła jego ważność. Zdecydowanie zalecamy używanie Biblioteki uwierzytelniania Microsoft (MSAL) w przypadku uzyskiwania tokenu dostępu. Ponadto błąd ten może pojawić się, jeśli próbujesz użyć delegowanego tokenu dostępu przyznanego dla konta osobistego Microsoft w celu uzyskania dostępu do interfejsu API, który obsługuje jedynie konta służbowe (konta organizacji).

**Błąd zabroniony 403: Czy wybrano prawidłowy zestaw uprawnień?**

Upewnij się, że żądano prawidłowego zestawu uprawnień opartego na interfejsach API programu Microsoft Graph wywoływanych przez Twoją aplikację. Zalecane uprawnienia z najniższym poziomem są zapewnione we wszystkich tematach metody referencyjnej dla interfejsu API programu Microsoft Graph. Ponadto uprawnienia te muszą być przyznane aplikacji przez użytkownika lub administratora. Przyznawanie uprawnień zazwyczaj odbywa się poprzez stronę zgody lub użycie bloku rejestracji aplikacji na Portalu Azure. Z poziomu bloku **Ustawienia** dla danej aplikacji kliknij pozycję **Wymagane uprawnienia**, a następnie kliknij pozycję **Udzielanie uprawnień**. Aby uzyskać więcej informacji, zobacz:

- [Uprawnienia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Opis uprawnień i zgody w usłudze Microsoft Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Błąd zabroniony 403: Czy Twoja aplikacja pozyskała token zgodny z wybranymi uprawnieniami?**

Upewnij się, że typy żądanych lub udzielonych uprawnień odpowiadają typowi tokenu dostępu, który Twoja aplikacja pozyskuje. Możesz żądać i udzielać uprawnień aplikacji, ale używać tokenów przepływów interakcyjnych delegowanych kodów zamiast tokenów przepływów poświadczeń klientów, bądź żądać lub udzielać delegowanych uprawnień, ale używać tokenów przepływów poświadczeń klientów zamiast tokenów przepływów delegowanych kodów.

W celu uzyskania dodatkowych informacji dotyczących pozyskiwania tokenów, zobacz:

- [Uzyskiwanie dostępu w imieniu użytkowników oraz delegowane uprawnienia](https://docs.microsoft.com/graph/auth-v2-user) 
- [Microsoft Azure Active Directory wer. 2.0 — przepływ kodu autoryzacji OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Uzyskiwanie dostępu bez uprawnień użytkownika (usługi demona) i aplikacji](https://docs.microsoft.com/graph/auth-v2-service) 
- [Microsoft Azure Active Directory wer. 2.0 — przepływ poświadczeń klienta OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Błąd zabroniony 403: resetowanie haseł**

Obecnie nie istnieją uprawnienia usługi demon dla uprawnień aplikacji między usługami, które umożliwiają resetowanie haseł użytkowników. Te interfejsy API są obsługiwane wyłącznie przy użyciu przepływów interakcyjnych delegowanych kodów z zalogowanym administratorem. Aby uzyskać więcej informacji, zobacz [Uprawnienia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**Zabroniony 403: Czy użytkownik ma dostęp i jest on licencjonowany?**

W przypadku przepływów delegowanych kodów program Microsoft Graph ocenia, czy żądanie jest dozwolone na podstawie uprawnień udzielonych aplikacji oraz uprawnień posiadanych przez zalogowanego użytkownika. Błąd ten zazwyczaj wskazuje, że użytkownik nie jest wystarczającego uprawniony do wykonania żądania **lub** użytkownik nie jest licencjonowany w zakresie danych, do których uzyskuje dostęp. Tylko użytkownicy z wymaganymi uprawnieniami lub licencjami mogą pomyślnie wykonać żądanie.

**Zabroniony 403: Czy wybrano poprawny interfejs API zasobu?**

Usługi interfejsu API, np. Microsoft Graph, sprawdzają, czy oświadczenie *odbiorcy* w odebranym tokenie dostępu odpowiada wartości, jakiej oczekuje dla siebie, a jeśli nie, występuje błąd zabroniony 403. Typową pomyłką powodującą wystąpienie tego błędu jest próba używania tokenu pozyskanego dla interfejsów API usługi Azure AD Graph, interfejsów API programu Outlook lub interfejsów API SharePoint/OneDrive do wywołania programu Microsoft Graph (lub na odwrót). Upewnij się, że zasób (lub zakres), dla którego Twoja aplikacja pozyskuje token, odpowiada interfejsowi API, który aplikacja wywołuje.

**Nieprawidłowe żądanie 400 lub Zabroniony 403: Czy użytkownik spełnia zasady dostępu warunkowego (CA) swojej organizacji?**

Na podstawie zasad dostępu warunkowego (CA) organizacji użytkownik uzyskujący dostęp do zasobów programu Microsoft Graph za pośrednictwem Twojej aplikacji może być wzywany do podania dodatkowych informacji, które nie są dostępne w tokenie dostępu, który pierwotnie pozyskała Twoja aplikacja. W takim przypadku Twoja aplikacja otrzyma **400 z błędem *interaction_required*** podczas pozyskiwania tokenu dostępu bądź **403 z błędem *insufficient_claims*** w przypadku wywoływania programu Microsoft Graph. W obu przypadkach odpowiedź dotycząca błędu zawiera dodatkowe informacje, które mogą być przedstawione autoryzowanemu punktowi końcowemu w celu wezwania użytkownika do podania dodatkowych informacji (np. w celu uwierzytelnienia wieloskładnikowego lub rejestracji urządzenia).

W celu uzyskania dodatkowych informacji dotyczących dostępu warunkowego, zobacz:

- [Obsługa wezwań dotyczących dostępu warunkowego przy użyciu biblioteki MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Wskazówki dla deweloperów w zakresie dostępu warunkowego usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Zakończenie świadczenia pomocy technicznej dla biblioteki Azure Active Directory Authentication Library (ADAL) oraz interfejsu API usługi Azure AD Graph (AAD Graph)_* _

- Począwszy od 30 czerwca 2020 r. nie będziemy już dłużej dodawać żądnych nowych funkcji do biblioteki Azure Active Directory Authentication Library (ADAL) oraz interfejsu API usługi AD Graph (AAD Graph). Będziemy nadal zapewniać pomoc techniczną i aktualizacje zabezpieczeń, natomiast nie będziemy dłużej dostarczać aktualizacji funkcji.
- Począwszy od 30 czerwca 2022 r. zakończymy świadczenie pomocy technicznej dla biblioteki ADAL i usługi AAD Graph, a także nie będziemy dłużej zapewniać pomocy technicznej lub aktualizacji zabezpieczeń.
    - Aplikacje używające biblioteki ADAL w istniejących wersjach systemu operacyjnego nadal będą działać po tej dacie, lecz nie będą uzyskiwać żadnej pomocy technicznej lub aktualizacji zabezpieczeń.
    - Aplikacje używające usługi AAD Graph po tej dacie mogą nie otrzymywać już dłużej odpowiedzi z punktu końcowego usługi AAD Graph.

_ *Migracja biblioteki ADAL**

Zalecamy zaktualizowanie do [Biblioteki uwierzytelniania Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), która oferuje najnowsze aktualizacje funkcji i zabezpieczeń. To zalecenie jest w kontekście firmy Microsoft migrującej swoje aplikacje do biblioteki MSAL do terminu ostatecznego zakończenia pomocy technicznej. Celem migracji aplikacji firmy Microsoft do biblioteki MSAL jest zapewnieniem że aplikacje będą korzystać z jej bieżących ulepszeń dotyczących zabezpieczeń i funkcji.

- [Przeczytaj sekcję ADAL — często zadawane pytania](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Dowiedz się na temat sposobu migracji aplikacji zależnie od platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Jeśli potrzebujesz pomocy w zrozumieniu, które aplikacje używają biblioteki ADAL, zalecamy przejrzenie kodu źródłowego wszystkich Twoich aplikacji i, w razie potrzeby, skontaktowanie się z dowolnym niezależnym dostawcą oprogramowania (ISV) lub dostawcą aplikacji. Pomoc techniczna firmy Microsoft może również dostarczyć listę aplikacji ADAL innych firm w Twojej dzierżawie.

**Migracja usługi AAD Graph**

W przypadku aplikacji używających usługi AAD Graph podstępuj zgodnie z naszymi wskazówkami w celu [migracji aplikacji usługi Azure AD Graph do programu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Nasz lista kontrolna dotycząca migracji stanowi punkt umożliwiający rozpoczęcie](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Portal rejestracji aplikacji Azure pokazuje, jakie aplikacje używają usługi AAD Graph. Zalecamy przejrzenie kodu źródłowego wszystkich Twoich aplikacji i, w razie potrzeby, skontaktowanie się z dowolnym dostawcą ISV lub dostawcą aplikacji. Pomoc techniczna firmy Microsoft może również udzielić informacji na temat użycia usługi AAD Graph w Twojej dzierżawie.

 











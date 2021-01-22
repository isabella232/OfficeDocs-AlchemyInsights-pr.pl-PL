---
title: Bezproblemowe problemy z logowaniem użytkownika logowania jednokrotnego
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935177"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Bezproblemowe problemy z logowaniem jednokrotnym użytkownika

Po uwierzytelnieniu użytkownika przeglądarka będzie buforować poświadczenia użytkownika, dzięki czemu w tej samej przeglądarce aplikacja automatycznie zaloguje się przy użyciu tego samego konta. Może to utrudnić indyjszemu użytkownikowi lub pojedynczeowi zalogowanie się do wielu kont na jednym urządzeniu. Aby rozwiązać ten problem: 1. Spróbuj zalogować się w innej przeglądarce. 2. Wyczyść pamięć podręczną przeglądarki i/lub pliki cookie i spróbuj zalogować się ponownie.

Jeśli nadal występują problemy z logowaniem, zalecamy, aby zdiagnozować i zautomatyzować kroki rozwiązywania problemów:

1. Zainstaluj rozszerzenie [My Apps Secure Browser Extension,](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) aby ułatwić korzystanie z usługi Azure Active Directory (Azure AD) w celu zapewnienia lepszej diagnostyki i rozwiązania podczas korzystania ze środowisk testowania w portalu Azure Portal.
2. Odtąd błąd można odtworzyć przy użyciu funkcji testowania na stronie konfiguracji aplikacji w portalu Azure Portal. Aby dowiedzieć się więcej, zobacz Debugowanie aplikacji logowania pojedynczego opartych [na programie SAML.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Jeśli używasz funkcji testowania w portalu Azure z rozszerzeniem My Apps Secure Browser Extension, możesz **pominąć krok 4.**
4. Aby otworzyć stronę konfiguracji logowania pojedynczego opartego na pliku SAML:
    - Otwórz portal [Azure i](https://portal.azure.com/) zaloguj się jako administrator **globalny lub** **coadmin.**
    - Otwórz rozszerzenie **usługi Azure Active Directory,** wybierając pozycję **Wszystkie** usługi w górnej części głównego lewego menu nawigacji.
    - Wpisz "Azure Active Directory" w polu wyszukiwania filtru i wybierz **element usługi Azure Active Directory.**
    - Wybierz **pozycję Aplikacje dla przedsiębiorstw** z menu nawigacji po lewej stronie w usłudze Azure Active Directory.
    - Wybierz **pozycję Wszystkie aplikacje,** aby wyświetlić listę wszystkich aplikacji. Jeśli nie widzisz tutaj aplikacji, którą chcesz wyświetlić, użyj kontrolki  Filtr u góry  listy Wszystkie aplikacje i ustaw opcję Pokaż na wartość **Wszystkie aplikacje.** 
    - Wybierz aplikację, którą chcesz skonfigurować do logowania pojedynczego.
    - Po ładowaniu aplikacji wybierz opcję **logowania** pojedynczego z menu nawigacji po lewej stronie.
    - Wybierz **pozycję Logowanie jednokrotne oparte na systemie SAML.**
5. Aby na podstawie tego błędu dowiedzieć się więcej o czynnościach zalecanych do obserwowania, zobacz Problemy z logowaniem się do aplikacji skonfigurowanych do logowania się pojedynczego opartego na systemie [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Aby rozwiązać inne problemy z logowaniem użytkowników, skorzystaj z następujących wskazówek:
    - [Protokół SAML Sign-On single](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Rozwiązywanie problemów z błędami podczas logowania się przy użyciu raportów usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Nieoczekiwany monit o zgodę](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Błąd zgody użytkownika](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problemy z logowaniem się z mojej aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Błąd na stronie logowania aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problem z logowaniem się do aplikacji Firmy Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)

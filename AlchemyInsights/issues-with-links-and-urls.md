---
title: Problemy z linkami i adresami URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054808"
---
# <a name="issues-with-links-and-urls"></a>Problemy z linkami i adresami URL

Identyfikator URI przekierowania/adres URL odpowiedzi (oba wyrażenia są używane zamiennie) są adresami URL używanymi przez platformę tożsamości Microsoft w celu zwracania tokenów wymaganych przez aplikację. Aby uzyskać informacje na temat tych adresów URL, zapoznaj się z następującymi artykułami:

- [Przepływy uwierzytelniania i scenariusze aplikacji](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) — informacje na temat identyfikatorów URI przekierowania na stronie **Rejestracja aplikacji** dla każdego scenariusza.
- [Ograniczenia i limity identyfikatora URI przekierowania/adresu URL odpowiedzi](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Nie wiem, jak zarejestrować prawidłowy identyfikator URI przekierowania/ adres URL odpowiedzi w przypadku mojej aplikacji**

Gdy logujesz się we wdrażanej aplikacji, jeśli w oknie dialogowym logowania jest wyświetlany kod **AADSTS50011: adres URL odpowiedzi określony w żądaniu jest niezgodny z adresami URL skonfigurowanym dla aplikacji <your app ID>**, musisz dodać identyfikator URI, który został użyty przez kod w żądaniu tokena dla platformy tożsamości Microsoft.

Aby dodać adres URL odpowiedzi, przejdź do karty **Uwierzytelnianie** na stronie **rejestracji aplikacji** w portalu Microsoft Azure Portal i dodaj wpis w sekcji **Identyfikatory URI przekierowania**. Wartość, jaką należy wprowadzić, zależy od typu tworzonej aplikacji zgodnie z poniższym opisem:

- W przypadku aplikacji typu Single Page Application i aplikacji internetowych, adres URL odpowiedzi jest adresem URL w Twojej aplikacji. Zobacz [Rejestracja aplikacji typu Single Page Application ](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) lub [Rejestrowanie aplikacji Web App za pomocą portalu Microsoft Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- W przypadku aplikacji klasycznych wartość, jaką należy wybrać, zależy od:
    - platformy (MacOS jest innym systemem niż Windows czy Linux),
    - sposobu uzyskiwania tokenu (interaktywnie, za pomocą przepływu kodu urządzenia, Zintegrowanego uwierzytelnienia systemu Windows [IWA] bądź nazwy użytkownika/hasła).
    W celu uzyskania szczegółowych informacji zobacz [aplikacje klasyczne — Rejestracja aplikacji — Identyfikator URI przekierowania](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- W przypadku aplikacji dla urządzeń przenośnych identyfikator URI przekierowania zależy od:
    - platformy (iOS/Android/UWP),
    - informacji używanych do tworzenia aplikacji, np. identyfikatora pakietu w systemie iOS, nazwy pakietu i skrótu podpisu w systemie Android. Rejestracja aplikacji portalu Microsoft Azure Portal będzie pomocna. W celu uzyskania szczegółowych informacji zobacz [Konfigurowanie platformy i identyfikatory URI przekierowania](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Interfejsy API sieci Web i niektóre dyskretne sposoby uzyskiwania tokenów (IWA i nazwa użytkownika/hasło) nie wymagają identyfikatora URI przekierowania.

**Wdrażam swoją aplikację internetową i gdy ją testuję, uzyuskuję komunikat o niezgodności adresu URL odpowiedzi**

Dodaj identyfikatory URI przekierowania w przypadku wszystkich lokalizacji, w których jest wdrażana aplikacja internetowa. Aby uzyskać więcej informacji, zobacz [Rejestrowanie aplikacji Web App za pomocą portalu Microsoft Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Dodaj identyfikator URI przekierowania dla lokalizacji niezwłocznie po wdrożeniu aplikacji w tej lokalizacji.

**Nie mogę zarejestrować wystarczającej liczby adresów URL odpowiedzi**

Jesteś niezależnym dostawcą oprogramowania i masz jeden lub kilka identyfikatorów URI dla każdego swojego klienta. Chcesz migrować z usługi ADAL/Azure AD wer. 1.0 do MSAL/platformy tożsamości Microsoft i została osiągnięta [maksymalna liczba identyfikatorów URI przekierowania](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Aby rozwiązać ten problem, [dodaj identyfikatory URI przekierowania do zasad usługi](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), które odpowiadają każdemu Twojemu klientowi.

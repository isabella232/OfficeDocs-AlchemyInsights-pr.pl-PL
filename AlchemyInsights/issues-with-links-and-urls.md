---
title: Problemy z łączami i adresami URL
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
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974749"
---
# <a name="issues-with-links-and-urls"></a>Problemy z łączami i adresami URL

Adresy URL przekierowania URI/zwrotów (oba wyrażenia są wymienne) to adresy URL używane przez platformę Microsoft Identity na potrzeby zwracania tokenów wymaganych przez aplikację. Aby uzyskać informacje na temat tych adresów URL, zobacz następujące artykuły:

- [Przepływy uwierzytelniania i scenariusze aplikacji](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) — informacje o identyfikatorach URI przekierowania na stronie **rejestracji aplikacji** dla każdego scenariusza.
- [Przekierowywanie ograniczeń i ograniczeń adresów URL w celu przekierowania URI/odpowiedzi](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Nie wiem, jak zarejestrować odpowiedni adres URL przekierowania/Odpowiedz na moją aplikację**

Po zalogowaniu się przy użyciu opracowywanej aplikacji, jeśli w oknie dialogowym logowania jest wyświetlany komunikat **AADSTS50011: adres URL odpowiedzi określony w żądaniu jest niezgodny z adresami URL odpowiedzi skonfigurowanymi dla <your app ID> aplikacji**, należy dodać do rejestracji aplikacji, identyfikator URI przekierowania, który został wykorzystany przez kod w żądaniu tokena na platformie Microsoft Identity.

Aby dodać adres URL odpowiedzi, przejdź do karty **uwierzytelnianie** na stronie **rejestracji aplikacji** w portalu Azure, a następnie Dodaj wpis w sekcji **przekierowanie identyfikatorów URI** . Identyfikatory URI przekierowania są wpisywane (sieć Web lub komórkowy/pulpit). Wartość, którą należy wprowadzić, zależy od typu konstruowanej aplikacji, zgodnie z opisem poniżej:

- W przypadku aplikacji jednostronicowych i aplikacji sieci Web adres URL odpowiedzi jest adresem URL w aplikacji. Wyświetlanie [jednostronicowej rejestracji aplikacji](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) lub [Rejestrowanie aplikacji aplikacji sieci Web za pomocą portalu Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- W przypadku aplikacji klasycznych wartość, którą należy wybrać, zależy od:
    - Platforma (MacOS jest różna od systemu Windows lub Linux)
    - sposób uzyskiwania tokenu (interaktywny, z funkcją przepływu kodu urządzenia) ze zintegrowanym uwierzytelnianiem systemu Windows [IWA] lub z nazwą użytkownika/hasłem).
    Aby uzyskać szczegółowe informacje, zobacz [aplikacje klasyczne — Rejestracja aplikacji — identyfikator URi przekierowania](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- W przypadku aplikacji mobilnych identyfikator URI przekierowania zależy od:
    - Platforma (iOS/Android/UWP)
    - informacje używane do tworzenia aplikacji, takie jak identyfikator pakietu w systemie iOS, oraz nazwa pakietu i skrót podpisu w systemie Android Rejestracja aplikacji Azure Portal pomoże Ci. Aby uzyskać szczegółowe informacje, zobacz temat [Konfiguracja platformy i identyfikatory URI przekierowania](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Interfejsy API sieci Web i niektóre z cichych metod pobierania tokenów (IWA i username/Password) nie wymagają identyfikatora URI przekierowania.

**Moja aplikacja sieci Web została wdrożona, a po przetestowaniu wdrożonej aplikacji otrzymuję komunikat o niezgodności adresu URL odpowiedzi**

Dodaj identyfikatory URI przekierowania dla wszystkich lokalizacji, w których ma zostać wdrożona aplikacja sieci Web. Aby uzyskać więcej informacji, zobacz [Rejestrowanie aplikacji sieci Web w witrynie Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Dodaj identyfikator URI przekierowania dla lokalizacji zaraz po wdrożeniu aplikacji w tej lokalizacji.

**Nie mogę zarejestrować zbyt małej liczby adresów URL odpowiedzi**

Jesteś dostawcą ISV i masz co najmniej jednego identyfikator URI przekierowania dla każdego klienta. Chcesz przeprowadzić migrację z usługi ADAL/Azure AD w wersji 1.0 do MSAL/Microsoft Identity platform i osiągnęłeś [maksymalną liczbę identyfikatorów URI przekierowania](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Aby to wyeliminować, [Dodaj identyfikatory URI przekierowania do podmiotów usług](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) , które odpowiadają każdemu z klientów.

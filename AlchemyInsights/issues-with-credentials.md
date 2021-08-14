---
title: Problemy z poświadczeniami
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
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986829"
---
# <a name="issues-with-credentials"></a>Problemy z poświadczeniami

Platforma tożsamości Microsoft przepływ poświadczeń klienta [protokołu OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisuje sposób bezpośrednio programowania przy użyciu przepływu udzielania poświadczeń klienta protokołu OAuth 2.0.

**Jak zarządzać poświadczeniami hasła lub certyfikatu aplikacji?**

W interfejsie wideo usługi Azure cli możesz użyć poświadczeń [aplikacji az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) w celu usunięcia, na liście lub zresetowania hasła lub poświadczeń certyfikatu aplikacji.

**Jak użytkownicy resetują swoje hasła?**

Użytkownicy muszą zarejestrować [się w celu samodzielnego](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) resetowania hasła, zanim będą oni mieli możliwość resetowania swoich haseł. Po zarejestrowaniu się użytkownik może wykonać instrukcje z tego artykułu, aby zresetować swoje [hasło: Resetowanie](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)hasła służbowego lub szkolnego.

**Jak użytkownicy mogą zmieniać swoje hasła?**

Użytkownicy mogą wykonać czynności opisane w tym artykule, aby zmienić swoje hasła: [Jak zmienić hasło.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Mogą też [zarządzać hasłami aplikacji na przykład w celu weryfikacji dwuetapowej.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mój użytkownik jest wyświetlany komunikat o błędzie podczas zmieniania lub resetowania hasła**

Ten link zawiera informacje o typowych problemach, które mogą się pojawić, gdy użytkownik próbuje zresetować swoje [hasło: typowe problemy i ich rozwiązania](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Mam problem z resetowaniem hasła użytkownika**

- Upewnij się, że masz uprawnienia do resetowania haseł. *Tylko administratorzy globalni, hasła i administratorzy użytkowników mogą resetować hasła użytkowników.* Administratorzy globalni mogą także resetować hasła innych administratorów uprzywilejowanych.

- Upewnij się, że rozumiesz wymagania dotyczące licencjonowania:

  - W organizacji musi być przypisana co najmniej jedna licencja:
    - **Użytkownicy tylko w chmurze** — Office 365 płatnej wersji SKU usługi Microsoft (O365) lub Azure AD Basic
    - **Użytkownicy chmury i/lub** lokalni — Azure AD — wersja Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)
    - Aby dowiedzieć się więcej o wymaganiach licencjonowania, zobacz Wymagania licencjonowania dotyczące samodzielnego resetowania hasła w usłudze [Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Aby zresetować hasło użytkownika, znajdź użytkownika w usłudze Azure AD. Następnie na ekranie podglądu tego użytkownika kliknij przycisk "resetuj hasło".

**Przycisk resetowania hasła jest wyszzarowany**

Nie masz uprawnień do **resetowania** haseł tego użytkownika. *Tylko administratorzy globalni, hasła i administratorzy użytkowników mogą resetować hasła użytkowników.* Administratorzy globalni mogą także resetować hasła innych administratorów uprzywilejowanych.

**Nie widzę bladego resetowania hasła**

Nie masz uprawnień do resetowania haseł. *Tylko administratorzy globalni, hasła i administratorzy użytkowników mogą resetować hasła użytkowników.* Administratorzy globalni mogą także resetować hasła innych administratorów uprzywilejowanych.

**Nie widzę lokalnej tarczy integracji w resetowaniu hasła**

- Lokalna tarcza integracji pojawia się tylko w środowiskach hybrydowych — co oznacza, że do manipulowania hasłami użytkowników lokalnych używasz funkcji zapisu hasła.

- To blade nie jest widać, jeśli:

  - Nie korzystasz z funkcji zapisu hasła
  - Występuje problem z instalacją/łącznością zapisu hasła
  - Występuje problem z instalacją/łącznością usługi Azure AD Połączenie
  - Aby uzyskać więcej kroków rozwiązywania problemów z zapisem hasła, zobacz [Rozwiązywanie problemów z pisaniem hasła](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Nie wiem, jak zresetować hasło użytkownika**

1. Zaloguj się do portalu Azure Portal jako odpowiedni administrator.
2. Przejdź do bloku **Użytkownicy i grupy,** a następnie wybierz **pozycję Wszyscy użytkownicy.**
3. Wybierz użytkownika z listy.
4. Dla wybranego użytkownika wybierz **pozycję Przegląd**, a następnie na pasku poleceń wybierz pozycję **Resetuj hasło**.
5. Wybierz przycisk **Resetuj** hasło i postępuj zgodnie z instrukcjami wyświetlanymi na ekranie.
    - Resetowanie jest wykonywane tylko za pośrednictwem **portalu Azure Portal** i obsługuje pisanie hasła.

**Zresetować hasło użytkownika lokalnego z portalu usługi Office 365 Admin lub aplikacji mobilnej Office 365 ale użytkownik nadal nie może się zalogować**

W tym portalu pisanie zwrotne hasła nie jest obsługiwane. Ponownie zresetuj hasło użytkownika w portalu Azure Portal.

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
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063683"
---
# <a name="issues-with-credentials"></a>Problemy z poświadczeniami

Platforma tożsamości firmy Microsoft i przepływ poświadczeń klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisują sposób uwierzytelniania bezpośrednio przy użyciu przepływu przyznawania poświadczeń klienta OAuth 2.0.

**Jak zarządzać poświadczeniami hasła lub certyfikatu aplikacji?**

W interfejsie logowania do usługi Azure możesz użyć poświadczeń [aplikacji az ad,](https://docs.microsoft.com/cli/azure/ad/app/credential) aby usunąć, utworzyć listę lub zresetować poświadczenia certyfikatu lub hasła aplikacji.

**Jak użytkownicy resetują swoje hasła?**

Użytkownicy muszą zarejestrować [się w celu samodzielnego](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) resetowania hasła, zanim będą oni mieli możliwość resetowania swoich haseł. Po zarejestrowaniu użytkownik może wykonać instrukcje z tego artykułu, aby zresetować swoje hasło: [zresetuj](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)swoje hasło służbowe.

**Jak moi użytkownicy zmieniają swoje hasła?**

Użytkownicy mogą wykonać czynności opisane w tym artykule, aby zmienić swoje hasła: [jak zmienić hasło.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Mogą oni również [zarządzać hasłami aplikacji w celu weryfikacji dwuetapowej.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mój użytkownik jest wyświetlany komunikat o błędzie podczas zmieniania lub resetowania hasła**

Ten link zawiera informacje o typowych problemach, które mogą wystąpić podczas próby zresetowania hasła przez [użytkownika: typowe problemy i ich rozwiązania](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Mam problem z resetowaniem hasła użytkownika**

- Upewnij się, że masz upoważnienie do resetowania haseł. *Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników.* Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.

- Upewnij się, że rozumiesz wymagania dotyczące licencjonowania:

  - W organizacji musi być przypisana co najmniej jedna licencja:
    - **Tylko użytkownicy w chmurze** — dowolna płatna usługa Office 365 (O365) lub usługa Azure AD Basic
    - **Użytkownicy chmury i/lub** lokalni — Azure AD Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)
    - Aby dowiedzieć się więcej o wymaganiach licencjonowania, zobacz Wymagania licencjonowania dotyczące samodzielnego resetowania hasła w [usłudze Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Aby zresetować hasło użytkownika, znajdź użytkownika w usłudze Azure AD. Następnie na ekranie podglądu tego użytkownika kliknij przycisk "resetuj hasło".

**Przycisk resetowania hasła jest wyszzarowany**

Nie masz uprawnień do **resetowania** haseł tego użytkownika. *Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników.* Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.

**Nie widzę bladego resetowania hasła**

Nie masz uprawnień do resetowania haseł. *Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników.* Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.

**W resetowaniu hasła nie widzę lokalnego bloku integracji**

- Lokalna tarcza integracji pojawia się tylko w środowiskach hybrydowych — co oznacza, że do manipulowania hasłami użytkowników lokalnych używasz funkcji zapisu hasła.

- Ten blok blokowy nie jest wyświetlony, jeśli:

  - Nie korzystasz z funkcji zapisu hasła
  - Występuje problem z instalacją/łącznością zapisu hasła
  - Występuje problem z instalacją/łącznością programu Azure AD Connect
  - Aby uzyskać więcej kroków rozwiązywania problemów z zapisem hasła, zobacz [Rozwiązywanie problemów z pisaniem hasła](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Nie wiem, jak zresetować hasło użytkownika**

1. Zaloguj się do portalu Azure Portal jako odpowiedni administrator.
2. Przejdź do bloku **Użytkownicy i grupy,** wybierz **pozycję Wszyscy użytkownicy.**
3. Wybierz użytkownika z listy.
4. Dla wybranego użytkownika wybierz pozycję **Przegląd,** a następnie na pasku poleceń wybierz pozycję **Resetuj hasło.**
5. Wybierz przycisk **Resetuj** hasło i postępuj zgodnie z instrukcjami wyświetlanymi na ekranie.
    - Resetowanie odbywa się tylko za pośrednictwem **portalu Azure Portal** i obsługuje pisanie hasła.

**Resetowanie hasła użytkownika lokalnego z portalu administracyjnego usługi Office 365 lub aplikacji mobilnej usługi Office 365, ale użytkownik nadal nie może się zalogować**

W tym portalu nie jest obsługiwane pisanie zwrotne hasła. Zresetuj ponownie hasło użytkownika w portalu Azure Portal.

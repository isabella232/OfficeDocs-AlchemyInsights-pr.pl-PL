---
title: Rozwiązywanie problemów z SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038968"
---
# <a name="troubleshoot-sspr"></a>Rozwiązywanie problemów z SSPR

**Mam problemy z konfiguracją resetowania hasła**

- Jeśli jesteś administratorem i szukasz sposobu włączenia funkcji samodzielnego resetowania hasła, zobacz Samouczek włączania [ustawień SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), aby skonfigurować resetowanie hasła dla organizacji. Możesz również zapoznać się z wymaganiami [licencyjnymi.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) W organizacji musi być przypisana co najmniej jedna licencja.
    - **Użytkownicy tylko w chmurze** — Office 365 płatnej wersji SKU usługi Microsoft (O365) lub Azure AD Basic
    - **Użytkownicy chmury i/lub** lokalni — Azure AD — wersja Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)
- Aby uzyskać dodatkowe pytania na temat samodzielnego resetowania hasła, zapoznaj się z często [zadawanymi pytaniami.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Wyświetlany jest komunikat o błędzie**

Zapoznaj się z tym artykułem, aby znaleźć typowe błędy i ich rozwiązania: Rozwiązywanie [problemów z samodzielnego resetowania hasła](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mam problem z moimi zasadami resetowania hasła**

- Jeśli zasady resetowania hasła nie zachowują się zgodnie z oczekiwaniami lub jeśli masz pytania dotyczące zasad resetowania hasła, zapoznaj się z tym artykułem: Zasady i ograniczenia dotyczące haseł w [programie Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Zasady resetowania hasła nie dotyczą administratorów. Firma Microsoft wymusza silne, domyślne zasady resetowania hasła z dwoma bramami dla dowolnej roli administratora platformy Azure. Upewnij się, że test używasz u użytkownika, który nie jest administratorem. Aby uzyskać więcej informacji na temat zasad resetowania ustawień administratora, zobacz ten artykuł: Różnice w [zasadach resetowania przez administratora.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Nie chcę, aby moi użytkownicy zarejestrowyli dodatkowe informacje zabezpieczające przy resetowaniu hasła**

Możesz wstępnie wypełnić dane (atrybuty poczty e-mail i telefonu) dla użytkowników za pomocą interfejsu API, programu PowerShell lub narzędzia Azure AD Połączenie. Aby dowiedzieć się, jak to przeczytać:

- [Wdrażanie resetowania hasła bez konieczności rejestrowania użytkowników](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Jakich danych używa resetowanie hasła](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Chcę, aby moi użytkownicy zarejestrli swoje dodatkowe informacje zabezpieczające przy resetowaniu hasła**

1. Zaleć użytkownikom zarejestrowanie swoich informacji zabezpieczających w celu samodzielnego resetowania hasła, przekieruj ich [do aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Po wypełnieniu danych przez użytkownika (przez użytkownika lub administratora) przekieruj go do usługi [aka.ms/sspr,](https://passwordreset.microsoftonline.com/) aby umożliwić użytkownikom resetowanie własnych haseł.
1. Jeśli użytkownicy nadal mają problemy, prawdopodobnie są to użytkownicy **federacyjni** lub synchronizowani **skróty** haseł. Oznacza to, że prawdopodobnie występuje problem z usługą zapisu hasła.
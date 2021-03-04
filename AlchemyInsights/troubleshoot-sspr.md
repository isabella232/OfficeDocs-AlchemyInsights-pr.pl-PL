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
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430219"
---
# <a name="troubleshoot-sspr"></a>Rozwiązywanie problemów z SSPR

**Mam problem z konfiguracją resetowania hasła**

- Jeśli jesteś administratorem i szukasz sposobu włączenia funkcji samodzielnego resetowania hasła, zobacz samouczek "Włączanie [programu SSPR"](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)w celu skonfigurowania resetowania hasła dla organizacji. Możesz również zapoznać się z wymaganiami [licencjonowania.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) W organizacji musi być przypisana co najmniej jedna licencja.
    - **Tylko użytkownicy w chmurze** — dowolna płatna usługa Office 365 (O365) lub usługa Azure AD Basic
    - **Użytkownicy chmury i/lub** lokalni — Azure AD Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)
- Aby uzyskać dodatkowe pytania dotyczące samodzielnego resetowania hasła, zapoznaj się z [często zadawanymi pytaniami.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Wyświetlany jest komunikat o błędzie**

Zapoznaj się z tym artykułem, aby znaleźć typowe błędy i ich rozwiązania: Rozwiązywanie [problemów z samodzielnego resetowania hasła](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mam problem z zasadami resetowania hasła**

- Jeśli zasady resetowania haseł nie zachowują się zgodnie z oczekiwaniami lub masz pytania dotyczące zasad resetowania haseł, zapoznaj się z tym artykułem: Zasady i ograniczenia dotyczące haseł w usłudze [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Zasady resetowania haseł nie dotyczą administratorów. Firma Microsoft wymusza silne, domyślne zasady resetowania hasła z dwiema bramami dla dowolnej roli administratora platformy Azure. Upewnij się, że test używasz z użytkownikiem, który nie jest administratorem. Aby uzyskać więcej informacji na temat zasad resetowania konta administratora, zobacz ten artykuł: Różnice między [zasadami resetowania przez administratora.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Nie chcę, aby moi użytkownicy zarejestrowyli dodatkowe informacje zabezpieczające przy resetowaniu hasła**

Możesz wstępnie wypełnić dane (atrybuty poczty e-mail i telefonu) dla użytkowników za pomocą interfejsu API, programu PowerShell lub programu Azure AD Connect. Aby dowiedzieć się, jak to przeczytać:

- [Wdrażanie resetowania hasła bez konieczności rejestrowania użytkowników](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Jakie dane są używane przez resetowanie hasła](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Chcę, aby moi użytkownicy zarejestrują swoje dodatkowe informacje zabezpieczające w celu resetowania hasła**

1. Zachęć użytkowników do zarejestrowania swoich informacji zabezpieczających w celu samodzielnego resetowania hasła, przekieruj ich do [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Po wypełnieniu danych przez użytkownika (przez użytkownika lub administratora) [](https://passwordreset.microsoftonline.com/) przekieruj użytkownika do usługi aka.ms/sspr aby umożliwić użytkownikom resetowanie własnych haseł.
1. Jeśli użytkownicy nadal mają problemy, prawdopodobnie są to **użytkownicy federacyjni** lub zsynchronizowani **skrótami** haseł. Oznacza to, że prawdopodobnie występuje problem z usługą zapisu hasła.
---
title: Rozwiązywanie problemów z użytkownikami
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
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901333"
---
# <a name="announcements"></a>Pras

Postępuj zgodnie ze wskazówkami firmy Google dotyczącymi testowania zgodności, aby sprawdzić, czy aplikacja jest dotknięta zmianą. Porady firmy Google są dostępne w programie https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Upewnij się, że korzystasz z systemowego widoku WebView lub przeglądarki systemowej podczas podpisywania użytkowników za pomocą kont Google Google. Aby uzyskać więcej informacji, zobacz [problemy z logowaniem się do aplikacji tylko za pomocą przeglądarki Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Nie można utworzyć nowego użytkownika w katalogu usługi Azure AD**

Aby rozwiązać problem polegający na tym, że nie można utworzyć nowego użytkownika w usłudze Azure AD, wykonaj następujące czynności:

1. Upewnij się, że masz autoryzację do tworzenia nowego użytkownika standardowego. Tylko rola administratora globalnego lub administratora użytkowników w usłudze Azure Active Directory (AD) może utworzyć nowego użytkownika standardowego. Jeśli nie korzystasz z jednej z tych ról, poproś administratora o dodanie do jednej z tych ról lub utworzenia nowego konta użytkownika.
2. Upewnij się, że nazwa użytkownika znajduje się w domenie zweryfikowanej w usłudze Azure AD. Jeśli nie masz żadnych zweryfikowanych niestandardowych nazw domen w usłudze Azure AD, możesz użyć początkowej domeny usługi Azure AD, która kończy się na *. onmicrosoft.com.
3. Upewnij się, że nazwa użytkownika znajduje się w domenie, która nie jest federacyjnym użytkownikiem usługi Azure AD z lokalnej usługi AD. Użytkownicy nie mogą być dodawani do chmury przy użyciu nazw domen federacyjnych lokalnie.
4. Upewnij się, że żaden inny użytkownik lub kontakt nie ma już nazwy użytkownika, którą chcesz przypisać nowemu użytkownikowi. Nazwy użytkowników muszą być unikatowe w usłudze Azure AD.
5. Zobacz [role i Administratorzy usługi Azure](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) AD dla usługi Azure AD.
6. Zobacz [nazwy domen](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) usługi Azure AD.
7. Przejrzyj [dzienniki inspekcji](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) , aby uzyskać bardziej szczegółowe informacje na temat ostatnio utworzonych lub usuniętych użytkowników, takich jak wykonywanie akcji i kiedy.
8. Aby uzyskać więcej informacji na temat dodawania nowych użytkowników, zobacz [Tworzenie nowego użytkownika w usłudze Azure AD przy użyciu witryny Azure Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Aby uzyskać więcej informacji na temat uprawnień roli administratora w usłudze Azure AD, zobacz [role administracyjne usługi Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Aby uzyskać szczegółowe informacje na temat tworzenia użytkownika za pomocą programu Azure AD PowerShell, zobacz [usługa Azure AD PowerShell w celu utworzenia nowego użytkownika](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problem dotyczący tworzenia konta samoobsługowego**

Aby rozwiązać problemy dotyczące tworzenia konta samoobsługowego, wykonaj następujące czynności:

1. Aby korzystać z samoobsługowego tworzenia konta w aplikacjach, najpierw włącz samoobsługowe Tworzenie konta w dzierżawie. 
2. Aby umożliwić aplikacji obsługiwanie konta samoobsługowego, Dodaj je do przepływu użytkownika. Gdy następnym razem przejdziesz do strony logowania dla tej aplikacji, zobaczysz opcję **_bez konta? Utwórz je!_* _. Spowoduje to uruchomienie samoobsługowego procesu tworzenia konta.
3. Aby uzyskać informacje na temat korzystania z konta samoobsługowego w celu wypełniania organizacji w usłudze Azure AD, zobacz Tworzenie konta samoobsługowego w usłudze [Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Po skojarzeniu przepływu użytkownika z co najmniej jednym użytkownikiem użytkownicy, którzy odwiedzają tę aplikację, będą mogli utworzyć konto gościa, korzystając z opcji skonfigurowanych w przepływie użytkownika. Aby uzyskać więcej informacji na temat rejestrowania i uzyskiwania konta gościa, użytkownicy będą mogli wyświetlać samoobsługowe [Tworzenie konta dla użytkowników Gość](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

*Problem z zazapraszaniem użytkownika zewnętrznego**

Aby rozwiązać problemy dotyczące zapraszania użytkownika zewnętrznego, wykonaj następujące czynności:

Upewnij się, że wysyłasz zaproszenie użytkownika na adres e-mail, który jest zgodny z nazwą, w której użytkownik się loguje. Jeśli wyślesz zaproszenie na adres e-mail użytkownika serwera proxy, użytkownik nie może go zrealizować. Aby uzyskać więcej informacji, zobacz [dokumentację usługi Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Nie mogę przypisać licencji do użytkownika**

Aby rozwiązać problemy dotyczące przypisywania licencji do użytkownika, wykonaj następujące czynności:

1. Aby zarządzać licencjami użytkowników, upewnij się, że korzystasz z konta z jednym z wymaganych ról administratora: Administrator globalny, administrator licencji lub administrator użytkowników. Możesz sprawdzić rolę użytkownika na karcie **rola w katalogu** w bloku użytkownika.
2. Jeśli korzystasz z portalu Azure, a przydział licencji kończy się niepowodzeniem, kliknij powiadomienie w prawym górnym rogu. Spowoduje to otwarcie bloku ze szczegółami dotyczącymi tego, co poszło źle. W większości przypadków wystarczy zrozumieć i rozwiązać problem.
3. Aby można było przypisać licencję do użytkownika, upewnij się, że właściwość **Lokalizacja użycia** jest ustawiona dla tego użytkownika. Sprawdź, czy użytkownik ma tę właściwość ustawioną przez wyświetlenie karty **profil** w bloku użytkownika.
4. Upewnij się, że jest dostępna wystarczająca liczba licencji dla produktu, który próbujesz przypisać. Liczbę dostępnych licencji można zobaczyć w portalu Azure, w usłudze [Azure Active Directory — licencje > — > wszystkich produktów](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Użytkownik może już mieć inną licencję, której usługi są w konflikcie z osobami w nowej licencji, którą chcesz przypisać. Jeśli na przykład użytkownik ma włączoną usługę Exchange Online (plan 1), nie będzie można przypisać licencji z usługą Exchange Online (plan 2). Wyłączenie jednej z usług, aby zezwolić na nowe przypisanie licencji. Jeśli korzystasz z usługi Azure Portal lub poleceń cmdlet programu PowerShell, na stronie **Szczegóły problemu** jest wyświetlana lista określonych usług powodujących konflikt.
6. Jeśli próbujesz usunąć licencję, a kończy się niepowodzeniem, użytkownik może korzystać z innych licencji za pomocą usług, które są zależne od usług, które próbujesz usunąć. W przypadku korzystania z poleceń cmdlet usługi Azure Portal lub programu PowerShell w komunikacie o błędzie zostanie wystawiona lista określonych usług mających zależności.
7. Jeśli chcesz się dowiedzieć, dlaczego licencja została dodana/usunięta przez użytkownika (na przykład, kto inny w organizacji może wprowadzić zmiany), Sprawdź dzienniki inspekcji. Ustaw filtr na **działania dotyczące licencji** , aby pokazać wszystkie modyfikacje, w tym "aktor", który je wykonał.
8. Jeśli korzystasz z usługi Exchange Online, niektóre konta użytkowników w dzierżawie mogą być niepoprawnie skonfigurowane z tą samą wartością adresu serwera proxy. W takich przypadkach mogą być wyświetlane komunikaty o błędach ogólnych, gdy operacja licencji nie powiedzie się. [Ten artykuł](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) zawiera więcej informacji na temat tego problemu, w tym informacje na temat [łączenia się z usługą Exchange Online przy użyciu zdalnego programu PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Aby określić, którzy użytkownicy w dzierżawie mają ten sam adres proxy, uruchom polecenie cmdlet usługi Exchange Online:

Działał

Get-Recipient | gdzie {$ _. EmailAddresses-Match <user principal name> } | Nazwa fL, adresat, EmailAddresses






---
title: Problem z resetowaniem hasła
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039976"
---
# <a name="problems-resetting-password"></a>Problemy z resetowaniem hasła

Poniżej przedstawiono niektóre problemy, które mogą wystąpić podczas resetowania hasła, i możliwe rozwiązania:

**Mam problem z resetowaniem hasła, które nie jest uwzględnione w innych kategoriach**

- Upewnij się, że masz autoryzację do resetowania haseł. Tylko administratorzy globalni, hasła i administratorzy użytkowników mogą resetować hasła użytkowników. Administratorzy globalni mogą także resetować hasła innych administratorów uprzywilejowanych.
- Upewnij się, że rozumiesz wymagania dotyczące licencjonowania:
    - W organizacji musi być przypisana co najmniej jedna licencja
        - Użytkownicy tylko w chmurze — Office 365 płatnej wersji SKU usługi (O365) lub Azure AD Basic
        - Użytkownicy chmury i(lub) lokalni — Azure AD — wersja Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)
        - Aby dowiedzieć się więcej o wymaganiach licencjonowania, zobacz artykuł Wymagania licencjonowania dotyczące samodzielnego resetowania hasła w usłudze [Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mam problemy z testowaniem ustawionych przeze mnie zasad resetowania hasła**

- Ostatnio zastosowane zasady mogą potrwać kilka minut, aby zreplikować je we wszystkich centrach danych i punktach końcowych. Odległość fizyczna od centrum danych ma również wpływ na to, jak szybko są stosowane zmiany.
- Przetestuj z użytkownikiem końcowym, a nie administratorem, i przetestuj z niewielkim zestawem użytkowników. Zasady skonfigurowane w portalu Azure Portal mają zastosowanie TYLKO do użytkowników końcowych, a nie administratorów. Firma Microsoft wymusza silne, domyślne zasady resetowania hasła z dwoma bramami dla dowolnej roli administratora platformy Azure (na przykład administrator globalny, administrator pomocy technicznej, administrator haseł itp.).
    - Dowiedz się więcej o [zasadach dla administratorów.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Chcę wdrożyć resetowanie hasła, ale nie chcę, aby moi użytkownicy rejestrować dodatkowe informacje zabezpieczające**

Wstępnie wypełnij dane użytkowników, aby ich nie trzeba było. — Jako administrator możesz ustawić właściwości telefonu i poczty e-mail dla użytkowników przed rozpoczęciem resetowania hasła w Twojej organizacji. Możesz to zrobić przy użyciu interfejsu API, programu PowerShell lub usługi Azure AD Połączenie. Więcej informacji znajdziesz tutaj:
- [Wdrażanie resetowania hasła bez konieczności rejestrowania użytkowników](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Jakich danych używa resetowanie hasła](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Przycisk resetowania hasła jest wyszzarowany**

Nie masz uprawnień do resetowania haseł tego użytkownika. Tylko administratorzy globalni, hasła i administratorzy użytkowników mogą resetować hasła użytkowników. Administratorzy globalni mogą także resetować hasła innych administratorów uprzywilejowanych.

**Nie widzę bladego resetowania hasła**

Nie masz uprawnień do resetowania haseł. Tylko administratorzy globalni, hasła i administratorzy użytkowników mogą resetować hasła użytkowników. Administratorzy globalni mogą także resetować hasła innych administratorów uprzywilejowanych.

**Nie widzę lokalnej tarczy integracji w resetowaniu hasła**

- Lokalna tarcza integracji pojawia się tylko w środowiskach hybrydowych — co oznacza, że do manipulowania hasłami użytkowników lokalnych używasz funkcji zapisu hasła.
- To blade nie jest widać, jeśli:
    - Nie korzystasz z funkcji zapisu hasła
    - Występuje problem z instalacją/łącznością zapisu hasła
    - Występuje problem z instalacją/łącznością usługi Azure AD Połączenie
    - Aby uzyskać więcej kroków rozwiązywania problemów z zapisem hasła, zobacz sekcję Rozwiązywanie [problemów z pisaniem hasła](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nie wiem, jak zresetować hasło użytkownika**

1. Zaloguj się do portalu Azure Portal jako odpowiedni administrator.
1. Przejdź do bloku Użytkownicy i grupy, a następnie wybierz **pozycję Wszyscy użytkownicy.**
1. Wybierz użytkownika z listy.
1. Dla wybranego użytkownika wybierz **pozycję Przegląd**, a następnie na pasku poleceń kliknij pozycję **Resetuj hasło**.
1. Postępuj zgodnie z instrukcjami wyświetlanymi na ekranie.
    - Resetowanie jest wykonywane tylko za pośrednictwem portalu Azure Portal i obsługuje pisanie hasła.

**Zresetować hasło użytkownika lokalnego z portalu usługi Office 365 Admin lub aplikacji mobilnej Office 365 ale użytkownik nadal nie może się zalogować**

W tym portalu pisanie zwrotne hasła nie jest obsługiwane. Ponownie zresetuj hasło użytkownika w portalu Azure Portal — portal.azure.com


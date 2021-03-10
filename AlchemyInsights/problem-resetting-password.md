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
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696273"
---
# <a name="problems-resetting-password"></a>Problemy z resetowaniem hasła

Poniżej przedstawiono niektóre problemy, które mogą wystąpić podczas resetowania hasła i możliwe rozwiązania:

**Mam problem z resetowaniem hasła, które nie jest uwzględnione w innych kategoriach**

- Upewnij się, że masz upoważnienie do resetowania haseł. Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników. Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.
- Upewnij się, że rozumiesz wymagania dotyczące licencjonowania:
    - W organizacji musi być przypisana co najmniej jedna licencja
        - Tylko użytkownicy w chmurze — dowolna płatna usługa Office 365 (O365) lub usługa Azure AD Basic
        - Użytkownicy chmury i/lub lokalni — Azure AD Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)
        - Aby dowiedzieć się więcej o wymaganiach licencjonowania, zobacz artykuł Wymagania licencjonowania dotyczące samodzielnego resetowania hasła w [usłudze Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mam problemy z testowaniem ustawionych przeze mnie zasad resetowania hasła**

- Replikowanie ostatnio zastosowanych zasad we wszystkich centrach danych i punktach końcowych może potrwać kilka minut. Odległość fizyczna od centrum danych ma również wpływ na sposób szybkiego stosowania zmian.
- Przetestuj z użytkownikiem końcowego, a nie z administratorem, i przetestuj z niewielkim zestawem użytkowników. Zasady skonfigurowane w portalu Azure Portal mają zastosowanie TYLKO do użytkowników końcowych, a nie administratorów. Firma Microsoft wymusza silne, domyślne zasady resetowania hasła w dwóch bramach dla dowolnej roli administratora platformy Azure (przykład: Administrator globalny, Administrator pomocy technicznej, Administrator haseł itp.).
    - Dowiedz się więcej o [zasadach dla administratorów.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Chcę wdrożyć resetowanie hasła, ale nie chcę, aby moi użytkownicy rejestrować dodatkowe informacje zabezpieczające**

Wstępnie wypełnij dane użytkowników, aby nie muszą tego zrobić! — Jako administrator możesz ustawić właściwości telefonu i poczty e-mail dla użytkowników przed rozpoczęciem resetowania hasła w organizacji. Możesz to zrobić przy użyciu interfejsu API, programu PowerShell lub programu Azure AD Connect. Więcej informacji tutaj:
- [Wdrażanie resetowania hasła bez konieczności rejestrowania użytkowników](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Jakie dane są używane przez resetowanie hasła](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Przycisk resetowania hasła jest wyszzarowany**

Nie masz uprawnień do resetowania haseł tego użytkownika. Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników. Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.

**Nie widzę bladego resetowania hasła**

Nie masz uprawnień do resetowania haseł. Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników. Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.

**W resetowaniu hasła nie widzę lokalnego bloku integracji**

- Lokalna tarcza integracji pojawia się tylko w środowiskach hybrydowych — co oznacza, że do manipulowania hasłami użytkowników lokalnych używasz funkcji zapisu hasła.
- Ten blok blokowy nie jest wyświetlony, jeśli:
    - Nie korzystasz z funkcji zapisu hasła
    - Występuje problem z instalacją/łącznością zapisu hasła
    - Występuje problem z instalacją/łącznością programu Azure AD Connect
    - Aby uzyskać więcej kroków rozwiązywania problemów z zapisem hasła, zobacz sekcję Rozwiązywanie problemów z [pisaniem hasła](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nie wiem, jak zresetować hasło użytkownika**

1. Zaloguj się do portalu Azure Portal jako odpowiedni administrator.
1. Przejdź do bloku Użytkownicy i grupy, wybierz **pozycję Wszyscy użytkownicy.**
1. Wybierz użytkownika z listy.
1. Dla wybranego użytkownika wybierz **pozycję Przegląd,** a następnie na pasku poleceń kliknij pozycję **Resetuj hasło.**
1. Postępuj zgodnie z instrukcjami wyświetlanymi na ekranie.
    - Resetowanie odbywa się tylko za pośrednictwem portalu Azure Portal i obsługuje pisanie hasła.

**Resetowanie hasła użytkownika lokalnego z portalu administracyjnego usługi Office 365 lub aplikacji mobilnej usługi Office 365, ale użytkownik nadal nie może się zalogować**

W tym portalu nie jest obsługiwane pisanie zwrotne hasła. Zresetuj ponownie hasło użytkownika w portalu Azure Portal — portal.azure.com


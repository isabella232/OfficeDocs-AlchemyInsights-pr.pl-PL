---
title: Włączanie zapisywania zwrotnego haseł w programie Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814022"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Włączanie zapisywania zwrotnego haseł w programie Azure AD Connect

Aby włączyć zapisywanie zwrotne dla samoobsługowego resetowania hasła, najpierw włącz opcję zapisywania zwrotnego haseł w programie Azure AD Connect. Wykonaj następujące kroki na serwerze Azure AD Connect:

1. Zaloguj się na serwerze Azure AD Connect i uruchom kreatora konfiguracji **Azure AD Connect**.
2. Na **Stronie głównej** kliknij przycisk **Konfiguruj**.
3. Na stronie **Zadania dodatkowe** wybierz pozycję **Dostosuj opcje synchronizacji**, a następnie kliknij przycisk **Dalej**.
4. Na stronie **Połącz z usługą Azure AD**, wprowadź poświadczenie administratora globalnego dla Twojej dzierżawy platformy Azure, a następnie kliknij przycisk **Dalej**.
5. Na stronach **Połącz katalogi** oraz **Domena/jednostka organizacyjna** kliknij przycisk **Dalej**.
6. Na stronie **Funkcje opcjonalne** zaznacz pole wyboru obok opcji **Zapisywanie zwrotne haseł** i kliknij przycisk **Dalej**.
7. Na stronie **Gotowy do konfiguracji** kliknij przycisk **Konfiguruj** i poczekaj aż proces się skończy.
8. Kiedy konfiguracja dobiegnie końca, naciśnij przycisk **Wyjdź**.

Gdy zapisywanie zwrotne zostało już włączone w programie Azure AD Connect, skonfiguruj funkcję samoobsługowego resetowania hasła (SSPR) w usłudze Azure AD do zapisywania zwrotnego.  Aby włączyć zapisywanie zwrotne haseł dla funkcji SSPR, wykonaj następujące kroki:

1. Zaloguj się w portalu Azure używając konta administratora globalnego.
2. Wyszukaj i wybierz usługę **Azure Active Directory**, kliknij przycisk **Resetowanie hasła**, a następnie kliknij przycisk **Integracja lokalna**.
3. Ustaw dla opcji **Zapisywać zwrotnie hasła w katalogu lokalnym?** wartość **Tak**.
4. Ustaw dla opcji **Zezwalać użytkownikom na odblokowanie konta bez resetowania hasła?** wartość **Tak**.
5. Po zakończeniu kliknij przycisk **Zapisz**.

Aby uzyskać więcej informacji, zobacz: [Włączanie zapisywania zwrotnego dla samoobsługowego resetowania hasła w usłudze Azure Active Directory w środowisku lokalnym](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)

> [!NOTE]
>  Gdy administrator resetuje hasło użytkownika w portalu Azure, jeśli jest to użytkownik federacyjny lub skrót hasła został zsynchronizowany, hasło zostanie zapisane zwrotnie lokalnie. Ta funkcja wymaga licencji Azure Premium (P1 lub P2) i obecnie nie jest obsługiwana w portalu Office Admin.

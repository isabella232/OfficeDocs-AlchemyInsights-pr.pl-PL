---
title: Synchronizacja haseł
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482041"
---
# <a name="password-synchronization"></a>Synchronizacja haseł

**Synchronizacja skrótów haseł w ogóle nie działa**

Niektóre typowe problemy napotykane przez klientów, gdy synchronizacja skrótów haseł nie działa:

- Konto usługi Active Directory używane przez usługę Azure AD Connect  do komunikowania się z lokalną usługą Active Directory nie jest udzielane uprawnień Do replikowania zmian w katalogu i replikowania zmian katalogu **Wszystkie** uprawnienia, które są wymagane do synchronizacji haseł — należy rozwiązać ten problem, udzielając tych uprawnień kontu usługi Active Directory.
- Synchronizacja skrótów haseł jest wyłączona po zmianie  przez administratora metody user Sign-In z synchronizacji haseł na inną opcję, taką jak  federacja z usługami **AD FS** w kreatorze Azure AD Connect — ten problem można rozwiązać, ponownie włączając funkcję synchronizacji skrótów haseł w kreatorze Azure AD Connect.
- Problem z łącznością z lokalną usługą Active Directory. Na przykład niektóre kontrolery domeny nie są dostępne [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) przez usługę Azure AD Connect lub wymagane porty są blokowane przez zaporę — należy rozwiązać ten problem, upewniając się, że łączność między serwerem Azure AD Connect a lokalną usługą Active Directory działa prawidłowo.
- Serwer Azure AD Connect jest obecnie w trybie tymczasowego, co spowoduje, że serwer nie będzie mógł uzyskać skrótów haseł — Aby rozwiązać ten problem, wykonaj czynności opisane w sekcji Rozwiązywanie problemów z synchronizacją haseł z synchronizacją programu [Azure AD Connect —](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)nie są synchronizowane żadne hasła.

**Synchronizacja skrótów haseł nie działa w przypadku niektórych użytkowników**

1. Jeśli zauważysz, że skrót haseł nie jest synchronizowany  dla użytkownika, użyj zadania rozwiązywania problemów w programie Azure AD Connect, aby zbadać i rozwiązać ten problem. Wykonaj następujące zadania:

    a. [Uruchamianie zadania rozwiązywania problemów w kreatorze](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Używanie polecenia cmdlet do rozwiązywania problemów w celu zbadania problemu z synchronizacją skrótów haseł dla określonego użycia](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Dla obiektu użytkownika lokalnej usługi Active Directory jest włączona opcja Użytkownik musi zmienić hasło **przy następnej** opcji logowania. Gdy ta opcja jest włączona, użytkownikowi jest przypisywane hasło tymczasowe i zostanie wyświetlony monit o zmianę hasła przy następnym loganiu. Program Azure AD Connect nie synchronizuje haseł tymczasowych z usługą Azure AD.

Aby rozwiązać powyższy problem, wykonaj jedną z następujących czynności:

- Poproś użytkownika o zalogowanie się do aplikacji lokalnej (na przykład aplikacji klasycznej systemu Windows) i zmianę hasła. Nowe hasło zostanie zsynchronizowane z usługą Azure AD.
- Niech administrator zaktualizuje hasło użytkownika bez włączania opcji Użytkownik musi zmienić hasło podczas następnego logowania **i** udostępnić nowe hasło użytkownikowi.

3. Obiekt użytkownika lokalnej usługi Active Directory **nie** jest poprawnie skonfigurowany do synchronizacji obiektów lub synchronizacji haseł. Aby rozwiązać ten problem, wykonaj czynności opisane w tece Rozwiązywanie problemów z synchronizacją skrótów haseł za [pomocą synchronizacji programu Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)








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
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960845"
---
# <a name="password-synchronization"></a>Synchronizacja haseł

**Synchronizacja skrótów haseł nie działa**

Niektóre typowe problemy napotykane przez klientów, gdy synchronizacja skrótów haseł nie działa:

- Konto usługi Active Directory używane przez usługę Azure AD Połączenie do  komunikowania się z lokalną usługą Active Directory nie ma uprawnień Replikuj zmiany w katalogu i Replikuj zmiany katalogu **Wszystkie** uprawnienia, które są wymagane do synchronizacji haseł — należy rozwiązać ten problem, udzielając tych uprawnień kontom usługi Active Directory.
- Synchronizacja skrótów haseł jest wyłączona, gdy administrator  zmienił metodę synchronizacji haseł użytkownika Sign-In na inną opcję, taką jak Federacja z usługami **AD FS** w kreatorze usługi Azure AD Połączenie — ten problem można rozwiązać, ponownie włączając funkcję synchronizacji skrótów haseł w kreatorze skrótów haseł usługi Azure AD Połączenie. 
- Problem z łącznością z lokalną usługą Active Directory. Na przykład niektóre kontrolery domeny nie są dostępne przez [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) usługę Azure AD Połączenie lub wymagane porty są zablokowane przez zaporę — należy rozwiązać ten problem, upewniając się, że łączność między serwerem usługi Azure AD Połączenie a lokalną usługą Active Directory działa prawidłowo.
- Serwer usługi Azure AD Połączenie jest obecnie w trybie tymczasowego konfiguracji, co spowoduje, że serwer nie będzie mógł uzyskać dostępu do skrótów haseł . Aby rozwiązać ten problem, wykonaj czynności opisane w sekcji Rozwiązywanie problemów z synchronizacją haseł z synchronizacją usługi [Azure AD Połączenie](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)— Synchronizacja haseł nie jest synchronizowana.

**Synchronizacja skrótów haseł nie działa w przypadku niektórych użytkowników**

1. Jeśli zauważysz, że skrót haseł nie jest synchronizowany  dla użytkownika, użyj zadania rozwiązywania problemów w usłudze Azure AD Połączenie zbadać i rozwiązać ten problem. Wykonaj następujące zadania:

    a. [Uruchamianie zadania rozwiązywania problemów w kreatorze](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Badanie problemu z synchronizacją skrótów haseł na potrzeby określonego użycia przy użyciu polecenia cmdlet rozwiązywania problemów](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Dla obiektu użytkownik usługi Active Directory w lokalnej usłudze Active Directory jest włączona zmiana hasła **przy następnej opcji** logowania. Gdy ta opcja jest włączona, użytkownikowi zostanie przypisane hasło tymczasowe i zostanie wyświetlony monit o zmianę hasła przy następnym loganiu. Usługa Azure AD Połączenie nie synchronizuje haseł tymczasowych z usługą Azure AD.

Aby rozwiązać powyższy problem, wykonaj jedną z następujących czynności:

- Poproś użytkownika o zalogowanie się do aplikacji lokalnej (na przykład Windows) i zmianę hasła. Nowe hasło zostanie zsynchronizowane z usługą Azure AD.
- Niech administrator zaktualizuje hasło użytkownika bez włączania opcji Użytkownik musi zmienić hasło przy następnym **logie** i udostępnić nowe hasło użytkownikowi.

3. Lokalnych obiektów użytkowników usługi Active Directory **nie** skonfigurowano poprawnie do synchronizacji obiektów i synchronizacji haseł. Aby rozwiązać ten problem, wykonaj czynności opisane w tece Rozwiązywanie problemów z synchronizacją skrótów haseł z synchronizacją skrótów [Połączenie Azure AD.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)








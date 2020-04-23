---
title: Rozwiązywanie problemów z synchronizacją haseł
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732520"
---
# <a name="troubleshoot-password-synchronization"></a>Rozwiązywanie problemów z synchronizacją haseł

Aby rozwiązać problemy, w których żadne hasła nie są synchronizowane z usługą Azure AD Connect w wersji 1.1.614.0 lub nowszej:
  
1. Otwórz nową sesję programu Windows PowerShell na serwerze usługi Azure AD Connect z opcją **Uruchom jako administrator.**

2. Uruchom **Set-ExecutionPolicy RemoteSigned** lub **Set-ExecutionPolicy Unrestricted**.

3. Uruchom kreatora usługi Azure AD Connect.

4. Przejdź do strony **Zadania dodatkowe,** wybierz pozycję **Rozwiązywanie problemów**i kliknij przycisk **Dalej**.

5. Na stronie Rozwiązywanie problemów kliknij przycisk **Uruchom, aby uruchomić** menu rozwiązywania problemów w programie PowerShell.

6. W menu głównym wybierz pozycję **Rozwiązywanie problemów z synchronizacją haseł**.

7. W menu podrzędnym wybierz opcję **Synchronizacja haseł w ogóle nie działa**.

**Opis wyników zadania rozwiązywania problemów**
  
Zadanie rozwiązywania problemów wykonuje następujące kontrole:
  
- Sprawdza, czy funkcja synchronizacji haseł jest włączona dla dzierżawy usługi Azure AD.

- Sprawdza, czy serwer usługi Azure AD Connect nie jest w trybie przemieszczania.

- Dla każdego istniejącego lokalnego łącznika usługi Active Directory (który odpowiada istniejącemu lasowi usługi Active Directory):

- 
  - Sprawdza, czy funkcja synchronizacji haseł jest włączona.

  - Wyszukuje zdarzenia pulsu synchronizacji haseł w dziennikach zdarzeń aplikacji systemu Windows.

  - Dla każdej domeny usługi Active Directory w ramach lokalnego łącznika usługi Active Directory:

  - Sprawdza, czy domena jest osiągalna z serwera usługi Azure AD Connect.

  - Sprawdza, czy konta Usług domenowych Active Directory (AD DS) używane przez lokalny łącznik usługi Active Directory mają poprawną nazwę użytkownika, hasło i uprawnienia wymagane do synchronizacji haseł.

Aby uzyskać więcej pomocy w rozwiązywaniu problemów z synchronizacją haseł, zobacz [Rozwiązywanie problemów z synchronizacją haseł za pomocą synchronizacji usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  
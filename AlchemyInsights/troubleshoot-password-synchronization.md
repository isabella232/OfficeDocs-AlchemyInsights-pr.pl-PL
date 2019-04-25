---
title: Rozwiązywanie problemów z synchronizacją haseł
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390447"
---
# <a name="troubleshoot-password-synchronization"></a>Rozwiązywanie problemów z synchronizacją haseł

Aby rozwiązać problemy, których hasła nie są zsynchronizowane z Azure AD Connect w wersji 1.1.614.0 lub nowszej:
  
1. Otwórz sesję środowiska Windows PowerShell na serwerze Azure Połącz AD za pomocą opcji **Uruchom jako Administrator** . 
    
2. Uruchom **zestaw ExecutionPolicy RemoteSigned** lub **zestaw ExecutionPolicy Unrestricted**. 
    
3. Uruchom kreatora Połącz AD Azure.
    
4. Przejdź do ** dodatkowe zadania ** wybierz ** Rozwiązywanie ** i kliknij przycisk **Dalej**. 
    
5. Na stronie Rozwiązywanie problemów kliknij przycisk **Uruchom, aby uruchomić Rozwiązywanie problemów** menu w programie PowerShell. 
    
6. W menu głównym wybierz **Rozwiązywanie problemów z synchronizacją haseł**. 
    
7. W podmenu wybierz **Synchronizacja haseł nie działać wcale**. 
    
 **Zrozumieć wyniki zadań rozwiązywania problemów**
  
Zadania dotyczące rozwiązywania problemów, wykonuje następujące kontrole:
  
- Sprawdza, czy funkcja synchronizacji hasła jest włączona dla dzierżawy usługi Azure AD.
    
- Sprawdza, czy serwer Azure Połącz AD nie jest w trybie tymczasowej.
    
- Dla każdego istniejącego lokalnego łącznika usługi Active Directory (która odnosi się do istniejącego lasu usługi Active Directory):
    
- 
  - Walidacja będzie przeprowadzana, że włączona jest funkcja synchronizacji hasła.
    
  - Wyszukuje hasło synchronizacji pulsu zdarzenia w dzienniku zdarzeń aplikacji systemu Windows.
    
  - Dla każdej domeny usługi Active Directory w lokalnym łącznika usługi Active Directory:
    
  - Weryfikuje, że domena jest dostępne z serwera Azure Połącz AD.
    
  - Sprawdza, czy konta Usługi domenowe w usłudze Active Directory (AD DS), używane przez łącznik usługi Active Directory na lokalnym ma poprawną nazwę użytkownika, hasło i uprawnienia wymagane dla synchronizacji haseł.
    
Aby uzyskać pomoc, rozwiązywanie problemów z synchronizacji haseł zobacz [Rozwiązywanie problemów z synchronizacji haseł z Azure AD Connect synchronizacją](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  


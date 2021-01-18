---
title: Problem z łączeniem maszyn wirtualnych
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
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885666"
---
# <a name="issue-joining-vms"></a>Problem z łączeniem maszyn wirtualnych

Aby wyeliminować problemy występujące podczas próby dołączenia do maszyn wirtualnych, wykonaj następujące czynności:

1. Spróbuj zalogować się przy użyciu formatu **UPN** (na przykład "JoeUser@contoso.com") zamiast formatu **sAMAccountName** ("CONTOSO\joeuser").
2. Upewnij się, że włączono synchronizację haseł, zgodnie z instrukcjami przedstawionymi w przewodniku *wprowadzenie* .
3. Upewnij się, że konto użytkownika, którego dotyczy problem, nie jest kontem zewnętrznym w dzierżawie usługi Azure AD. Użytkownicy zewnętrzni nie mogą zalogować się w zarządzanej domenie, ponieważ usługi domenowe w usłudze Azure AD nie mają poświadczeń dla takich kont użytkowników.
4. Jeśli konto użytkownika, którego dotyczy problem, jest kontem użytkownika tylko w chmurze, upewnij się, że użytkownicy zmienili swoje hasło po włączeniu usług domenowych w usłudze Azure AD. Wykonanie tej czynności powoduje generowanie skrótów poświadczeń wymaganych do generowania usług domenowych w usłudze Azure AD.
5. Jeśli konta użytkowników, których dotyczy problem, są synchronizowane z katalogu lokalnego, upewnij się, że zalecana wersja usługi Azure AD Connect została skonfigurowana w celu przeprowadzania pełnej synchronizacji.
6. Jeśli po potwierdzeniu kroku 4 nadal występują problemy, wykonaj następujące polecenia na komputerze z synchronizacją:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.
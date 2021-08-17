---
title: Rozwiązywanie problemów z synchronizacją haseł
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105767"
---
# <a name="troubleshoot-password-synchronization"></a>Rozwiązywanie problemów z synchronizacją haseł

Aby rozwiązać problemy z synchronizacją haseł, zacznij od tego zadania rozwiązywania problemów Połączenie AAD w celu określenia, dlaczego synchronizacja haseł nie jest synchronizowana. Aby rozpocząć, przejdź do [zarządzania synchronizacją bezpośrednią.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Otwórz nową sesję Windows PowerShell na serwerze usługi Azure AD Połączenie i wybierz opcję **Uruchom jako administrator.**

2. Uruchom Set-ExecutionPolicy Signed remoteSigned lub Set-ExecutionPolicy Unrestricted (Nieograniczone).

3. Uruchom kreatora konfiguracji usługi Azure AD Połączenie usługi.

4. Przejdź na stronę Dodatkowe zadania i > **Rozwiązywanie**  >  **problemów Dalej.**

5. Wybierz **pozycję Uruchom,** aby otworzyć menu rozwiązywania problemów programu PowerShell.

6. Wybierz **pozycję Rozwiązywanie problemów z synchronizacją haseł.**

    Zazwyczaj problemem jest to, że hasło nie jest synchronizowane dla określonego konta użytkownika.

    **Notatki** Synchronizacja haseł kończy się niepowodzeniem, jeśli ostatnia pomyślna synchronizacja haseł została już jakiś czas temu.

Aby uzyskać więcej pomocy dotyczącej rozwiązywania problemów z synchronizacją haseł, zobacz Rozwiązywanie problemów z synchronizacją skrótów haseł z synchronizacją skrótów [Połączenie Azure AD.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)
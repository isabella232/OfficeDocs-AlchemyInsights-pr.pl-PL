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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664936"
---
# <a name="troubleshoot-password-synchronization"></a>Rozwiązywanie problemów z synchronizacją haseł

Aby rozwiązać problemy z synchronizacją haseł, zacznij korzystać z tego zadania rozwiązywania problemów z usługą AAD Connect w celu określenia, dlaczego hasła nie są synchronizowane. Aby rozpocząć, przejdź do obszaru [Zarządzanie synchronizacją bezpośrednią](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otwórz nową sesję programu Windows PowerShell na serwerze usługi Azure AD Connect, a następnie wybierz opcję **Uruchom jako administrator** .

2. Uruchom polecenie Set-ExecutionPolicy RemoteSigned lub Set-ExecutionPolicy bez ograniczeń.

3. Uruchom Kreatora usługi Azure AD Connect.

4. Przejdź do strony zadania dodatkowe > **rozwiązywania problemów**  >  **Next**.

5. Wybierz pozycję **Uruchom** , aby otworzyć menu Rozwiązywanie problemów z programem PowerShell.

6. Wybierz pozycję **Rozwiązywanie problemów z synchronizacją haseł**.

    Przyczyną problemu jest zwykle niezsynchronizowane hasło dla określonego konta użytkownika.

    **Uwagi** Synchronizacja haseł kończy się niepowodzeniem, jeśli Ostatnia pomyślna synchronizacja hasła była niedawna.

Aby uzyskać więcej pomocy dotyczącej rozwiązywania problemów z synchronizacją haseł, zobacz [Rozwiązywanie problemów z synchronizacją skrótu hasła za pomocą funkcji synchronizacji Azure](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)
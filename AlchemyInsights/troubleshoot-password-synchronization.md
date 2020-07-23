---
title: Rozwiązywanie problemów z synchronizacją haseł
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387887"
---
# <a name="troubleshoot-password-synchronization"></a>Rozwiązywanie problemów z synchronizacją haseł

Aby rozwiązać problemy z synchronizacją haseł, zacznij od użycia tego zadania rozwiązywania problemów AAD Connect, aby ustalić, dlaczego hasła nie są synchronizowane. Aby rozpocząć, przejdź do [zarządzania synchronizacją bezpośrednią](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otwórz nową sesję programu Windows PowerShell na serwerze usługi Azure AD Connect i wybierz opcję **Uruchom jako administrator.**

2. Uruchom Set-ExecutionPolicy RemoteSigned lub Set-ExecutionPolicy Unrestricted.

3. Uruchom kreatora usługi Azure AD Connect.

4. Przejdź do strony Zadania dodatkowe > **rozwiąż**  >  **dalej**.

5. Wybierz **przycisk Uruchom,** aby otworzyć menu rozwiązywania problemów z programem PowerShell.

6. Wybierz **pozycję Rozwiązywanie problemów z synchronizacją haseł**.

    Problem polega zazwyczaj na tym, że hasło nie jest synchronizowane dla określonego konta użytkownika.

    **Uwagi** Synchronizacja haseł kończy się niepowodzeniem, jeśli ostatnia pomyślna synchronizacja hasła miała jakiś czas temu.

Aby uzyskać więcej pomocy w rozwiązywaniu problemów z synchronizacją haseł, zobacz [Rozwiązywanie problemów z synchronizacją skrótów haseł z synchronizacją usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).
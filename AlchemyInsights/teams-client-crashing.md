---
title: Awarie klienta usługi Teams?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354062"
---
# <a name="teams-client-crashing"></a>Awarie klienta usługi Teams?

Jeśli masz problem z awariami klienta usługi Teams, spróbuj poniższych rozwiązań:

- Jeśli używasz aplikacji klasycznej Teams, [upewnij się, że aplikacja jest w pełni zaktualizowana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Upewnij się, że dostępne są wszystkie [adresy URL i zakresy adresów usługi Microsoft 365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)

- Zaloguj się przy użyciu konta administratora dzierżawy i sprawdź [pulpit nawigacyjny kondycji usługi,](https://docs.microsoft.com/office365/enterprise/view-service-health) aby sprawdzić, czy nie występuje awaria lub degradacja usługi.

- Odinstalowywanie i ponowne instalowanie aplikacji Teams (łącze)
    - Przejdź do folderu %appdata%\Microsoft\teams\ na komputerze i usuń wszystkie pliki w tym katalogu.
    - [Pobierz i zainstaluj aplikację Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), a jeśli to możliwe, zainstaluj teams jako administratora (kliknij prawym przyciskiem myszy instalator teams i wybierz "Uruchom jako administrator", jeśli jest dostępny).

Jeśli twój klient usługi Teams nadal ulega awarii, czy możesz odtworzyć problem? Jeśli tak:

1. Użyj rejestratora kroków, aby uchwycić swoje kroki.
    - Zamknij WSZYSTKIE niepotrzebne lub poufne aplikacje.
    - Uruchom rejestrator kroków i odtwórz problem po zalogowaniu się za pomocą konta użytkownika, którego dotyczy problem.
    - [Zbierz dzienniki zespołów, które przechwytują zarejestrowane kroki repro.](https://docs.microsoft.com/microsoftteams/log-files) **Uwaga:** Upewnij się, że przechwytujesz adres logowania użytkownika, którego dotyczy problem.
    - Zbieranie informacji o zrzucie i/lub zasobniku błędów (Windows). Uruchom program Windows Powershell na komputerze, na którym występuje awaria, i uruchom następujące polecenia:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Dołącz plik do sprawy pomocy technicznej.

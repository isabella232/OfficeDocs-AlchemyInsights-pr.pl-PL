---
title: Awarie klienta usługi Teams?
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826281"
---
# <a name="teams-client-crashing"></a>Awarie klienta usługi Teams?

Jeśli masz problem z awariami klienta usługi Teams, spróbuj poniższych rozwiązań:

- Jeśli używasz aplikacji klasycznej Teams, [upewnij się, że aplikacja jest w pełni zaktualizowana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Upewnij się, że wszystkie adresy URL i zakresy adresów platformy [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) są dostępne.

- Zaloguj się przy użyciu konta administratora dzierżawy i sprawdź pulpit [nawigacyjny](https://docs.microsoft.com/office365/enterprise/view-service-health) kondycji usługi, aby sprawdzić, czy nie występuje żadne uszkodzenie lub obniżenie wydajności usługi.

- Odinstalowanie i ponowne zainstalowanie aplikacji Teams (link)
    - Przejdź do folderu %appdata%\Microsoft\teams\ na komputerze i usuń wszystkie pliki w tym katalogu.
    - [Pobierz i zainstaluj aplikację Teams,](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)a jeśli to możliwe, zainstaluj aplikację Teams jako administrator (kliknij prawym przyciskiem myszy instalator Teams i wybierz opcję "Uruchom jako administrator", jeśli jest dostępny).

Jeśli klient usługi Teams nadal ulega awarii, czy możesz odtworzyć problem? Jeśli tak jest:

1. Skorzystaj z Rejestratora problemów, aby przechwycić czynności.
    - Zamknij WSZYSTKIE zbędne lub poufne aplikacje.
    - Uruchom Rejestratora problemów i odtprodukuj problem po zalogowaniu się przy użyciu odpowiedniego konta użytkownika.
    - [Zbierz dzienniki zespołów, które przechwytują zarejestrowane kroki ponownego przekierowy.](https://docs.microsoft.com/microsoftteams/log-files) **Uwaga:** upewnij się, że przechwycono adres logowania użytkownika, u który ma wpływ.
    - Zbierz zrzut i/lub informacje zasobnika błędów (Windows). Uruchom program Windows PowerShell na komputerze, na którym występuje awaria, i uruchom następujące polecenia:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Dołącz plik do sprawy pomocy technicznej.

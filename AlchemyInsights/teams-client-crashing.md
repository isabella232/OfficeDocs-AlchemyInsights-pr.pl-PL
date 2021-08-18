---
title: Teams awarie klienta
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
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321635"
---
# <a name="teams-client-crashing"></a>Teams awarie klienta

Jeśli masz problem z awariami klienta usługi Teams, spróbuj poniższych rozwiązań:

- Jeśli używasz aplikacji klasycznej Teams, [upewnij się, że aplikacja jest w pełni zaktualizowana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Upewnij się, że [wszystkie Microsoft 365 URL i zakresy adresów są](https://docs.microsoft.com/microsoftteams/connectivity-issues) dostępne.

- Zaloguj się przy użyciu konta administratora dzierżawy i sprawdź pulpit [nawigacyjny](https://docs.microsoft.com/office365/enterprise/view-service-health) kondycji usługi, aby sprawdzić, czy nie występuje żadne uszkodzenie lub obniżenie wydajności usługi.

- Odinstaluj i ponownie zainstaluj aplikację Teams.
    - Przejdź do folderu %appdata%\Microsoft\Teams\ na komputerze i usuń wszystkie pliki w tym katalogu.
    - [Pobierz i zainstaluj aplikację Teams,](https://www.microsoft.com/microsoft-teams/download-app)a jeśli to możliwe, zainstaluj aplikację Teams jako administrator (kliknij prawym przyciskiem myszy instalatora Teams i wybierz polecenie Uruchom jako **administrator,** jeśli jest dostępne).

Jeśli klient Teams nadal ulega awarii, spróbuj odtworzyć problem. Jeśli możesz:

1. Skorzystaj z Rejestratora problemów, aby przechwycić czynności.
    - Zamknij WSZYSTKIE zbędne lub poufne aplikacje.
    - Uruchom Rejestratora problemów i odtprodukuj problem po zalogowaniu się przy użyciu odpowiedniego konta użytkownika.
    - [Zbierz dzienniki zespołów, które przechwytują zarejestrowane kroki ponownego przekierowy.](https://docs.microsoft.com/microsoftteams/log-files) 
    
    **Uwaga:** Upewnij się, że przechwycono adres logowania użytkownika, u który ma wpływ.
    - Zbierz zrzut i/lub informacje zasobnika błędów (Windows). Uruchom Windows PowerShell na komputerze, na którym występuje awaria, i uruchom następujące polecenia (po każdym z poleceń naciśnij klawisz Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Po wygenerowaniu pliku tekstowego, który pojawi się na ekranie, zapisz go i dołącz do żądania usługi. 

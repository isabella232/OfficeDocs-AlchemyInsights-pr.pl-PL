---
title: Rozwiązywanie problemów z awariami usługi OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826209"
---
# <a name="troubleshoot-onedrive-crashes"></a>Rozwiązywanie problemów z awariami usługi OneDrive

Jeśli oneDrive wielokrotnie ulega awarii, spróbuj wykonać następujące kroki rozwiązywania problemów:

**Upewnij się, że klucze rejestru nie są ustawione:**

1. Za pomocą Edytora rejestru przejdź do HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Jeśli wartość DisableFileSyncNGSC jest ustawiona na 1, otwórz klucz i zmień wartość na 0.
3. Ręczne uruchamianie aplikacji OneDrive przez uruchomienie ![Naciśnij klawisz systemu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), wpisz OneDrive w polu wyszukiwania, a następnie kliknij aplikację komputerową OneDrive.

**Resetowanie aplikacji OneDrive:**

Uwagi:

- Zresetowanie aplikacji OneDrive powoduje odłączenie wszystkich istniejących połączeń synchronizacji (w tym twojej osobistej usługi OneDrive, jeśli je skonfiguruje).
- Zresetowanie aplikacji OneDrive na komputerze nie spowoduje utraty plików ani danych.

**Aby zresetować usługę OneDrive:**

1. Otwórz okno dialogowe Uruchamianie, naciskając klawisze Windows i R.
2. Wpisz %localappdata%\Microsoft\OneDrive\onedrive.exe /reset i naciśnij przycisk OK. Może zostać wyświetlone na krótko okno Polecenie.
3. Ręczne uruchamianie aplikacji OneDrive przez uruchomienie ![Naciśnij klawisz systemu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), wpisz OneDrive w polu wyszukiwania, a następnie kliknij aplikację komputerową OneDrive.

Uwagi:

- Jeśli przed zresetowaniu wybrano synchronizowanie tylko niektórych folderów, będzie konieczne ponowne ich zsynchronizowanie po ukończeniu synchronizacji. Przeczytaj [Wybieranie folderów usługi OneDrive do synchronizowania z komputerem, aby](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)uzyskać więcej   informacji.
- Musisz to zrobić w przypadku osobistej usługi OneDrive i OneDrive dla Firm.
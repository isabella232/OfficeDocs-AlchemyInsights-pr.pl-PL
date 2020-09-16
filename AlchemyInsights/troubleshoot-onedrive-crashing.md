---
title: Rozwiązywanie problemów z awariami usługi OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665008"
---
# <a name="troubleshoot-onedrive-crashes"></a>Rozwiązywanie problemów z awariami usługi OneDrive

Jeśli usługa OneDrive jest wielokrotnie awaria, spróbuj wykonać następujące czynności rozwiązywania problemów:

**Upewnij się, że klucze rejestru nie są ustawione:**

1. Korzystanie z edytora rejestru przejdź do HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Jeśli DisableFileSyncNGSC jest obecny i ustawiony na 1, Otwórz klucz i zmień wartość na 0.
3. Ręcznie uruchom usługę OneDrive, przechodząc do ekranu startowego ![Naciśnij klawisz systemu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)Wpisz OneDrive w polu wyszukiwania, a następnie kliknij aplikację klasyczną OneDrive.

**Resetowanie usługi OneDrive:**

Uwagi:

- Zresetowanie usługi OneDrive powoduje odłączenie wszystkich istniejących połączeń synchronizacji (łącznie z osobistą usługą OneDrive, jeśli została skonfigurowana).
- Nie utracisz plików lub danych przez zresetowanie usługi OneDrive na komputerze.

**Aby zresetować aplikację OneDrive:**

1. Otwórz okno dialogowe Uruchamianie, naciskając klawisze Windows i R.
2. Wpisz% LocalAppData% \Microsoft\OneDrive\onedrive.exe/Reset i naciśnij przycisk OK. Okno polecenia może być krótko wyświetlane.
3. Ręcznie uruchom usługę OneDrive, przechodząc do ekranu startowego ![Naciśnij klawisz systemu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)Wpisz OneDrive w polu wyszukiwania, a następnie kliknij aplikację klasyczną OneDrive.

Uwagi:

- Jeśli przed zresetowaniem wybrano opcję synchronizacji tylko niektóre foldery, konieczne będzie ponowne uruchomienie po zakończeniu synchronizacji. Aby uzyskać więcej informacji, zobacz [Wybieranie folderów usługi OneDrive, które mają być synchronizowane z komputerem](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .
- Musisz wykonać tę czynność dla swojej osobistej usługi OneDrive i usługi OneDrive dla firm.
---
title: Rozwiązywanie problemów z awariami usługi OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749164"
---
# <a name="troubleshoot-onedrive-crashes"></a>Rozwiązywanie problemów z awariami usługi OneDrive

Jeśli usługa OneDrive wielokrotnie ulega awarii, spróbuj wykonać następujące kroki rozwiązywania problemów:

**Upewnij się, że klucze rejestru nie są ustawione:**

1. Korzystając z Edytora rejestru, przejdź do HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Jeśli disableFileSyncNGSC jest obecny i ustawiony na 1, otwórz klucz i zmień wartość na 0.
3. Ręczne uruchamianie usługi OneDrive przez przejście do ekranu startowego ![Naciśnięcie klawisza Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), wpisz w polu wyszukiwania usługę OneDrive, a następnie kliknij aplikację klasyczną OneDrive.

**Resetowanie usługi OneDrive:**

Uwagi:

- Zresetowanie usługi OneDrive rozłącza wszystkie istniejące połączenia synchronizacji (w tym osobistą usługę OneDrive, jeśli jest skonfigurowana).
- Nie utracisz plików ani danych, resetując usługę OneDrive na komputerze.

**Aby zresetować usługę OneDrive:**

1. Otwórz okno dialogowe Uruchom, naciskając klawisze Windows i R.
2. Wpisz %localappdata%\Microsoft\OneDrive\onedrive.exe /reset i naciśnij przycisk OK. Okno polecenia może pojawić się krótko.
3. Ręczne uruchamianie usługi OneDrive przez przejście do ekranu startowego ![Naciśnięcie klawisza Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), wpisz w polu wyszukiwania usługę OneDrive, a następnie kliknij aplikację klasyczną OneDrive.

Uwagi:

- Jeśli wybrano synchronizację tylko niektórych folderów przed zresetowaniem, musisz to zrobić ponownie po zakończeniu synchronizacji. Przeczytaj [artykuł Wybierz foldery usługi OneDrive do synchronizacji z komputerem, aby](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)uzyskać więcej   informacji.
- Musisz to zrobić dla osobistej usługi OneDrive i usługi OneDrive dla Firm.
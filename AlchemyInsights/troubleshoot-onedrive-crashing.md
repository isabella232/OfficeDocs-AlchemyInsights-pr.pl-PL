---
title: Rozwiązywanie OneDrive awarii
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921017"
---
# <a name="troubleshoot-onedrive-crashes"></a>Rozwiązywanie OneDrive awarii

Jeśli OneDrive wielokrotnie ulega awarii, spróbuj wykonać następujące kroki rozwiązywania problemów:

**Upewnij się, że klucze rejestru nie są ustawione:**

1. Za pomocą Edytora rejestru przejdź do HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Jeśli wartość DisableFileSyncNGSC jest ustawiona na 1, otwórz klucz i zmień wartość na 0.
3. Ręczne uruchamianie OneDrive, przechodząc do przycisku Start ![Naciśnij klawisz Windows główne](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)wpisz OneDrive w polu wyszukiwania, a następnie kliknij aplikację OneDrive klasycznej.

**Resetowanie OneDrive:**

Uwagi:

- Zresetowanie OneDrive odłącza wszystkie istniejące połączenia synchronizacji (w tym osobiste konto OneDrive skonfigurowaniu).
- Zresetowanie ustawień komputera nie spowoduje utraty plików ani OneDrive danych.

**Aby zresetować OneDrive:**

1. Otwórz okno dialogowe Uruchamianie, naciskając klawisz Windows i klawisz R.
2. Wpisz %localappdata%\Microsoft\OneDrive\onedrive.exe /reset i naciśnij przycisk OK. Może zostać wyświetlone na krótko okno Polecenie.
3. Ręczne uruchamianie OneDrive, przechodząc do przycisku Start ![Naciśnij klawisz Windows główne](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)wpisz OneDrive w polu wyszukiwania, a następnie kliknij aplikację OneDrive klasycznej.

Uwagi:

- Jeśli przed zresetowaniu wybrano synchronizowanie tylko niektórych folderów, będzie konieczne ponowne ich zsynchronizowanie po ukończeniu synchronizacji. Przeczytaj [Wybieranie OneDrive synchronizowanych folderów z komputerem, aby](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)uzyskać więcej   informacji.
- Musisz wykonać te zadania na potrzeby osobistego OneDrive i OneDrive dla Firm.
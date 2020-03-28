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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030678"
---
# <a name="teams-client-crashing"></a>Awarie klienta usługi Teams?

Jeśli masz problem z awariami klienta usługi Teams, spróbuj poniższych rozwiązań:

- Jeśli używasz aplikacji klasycznej Teams, [upewnij się, że aplikacja jest w pełni zaktualizowana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Upewnij się, że wszystkie [ zakresy adresów URL i adresy URL pakietu Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) są dostępne.

- Zaloguj się do konta administratora usługi i sprawdź na [pulpicie nawigacyjnym kondycji usługi](https://docs.microsoft.com/office365/enterprise/view-service-health), czy nie ma awarii ani obniżenia wydajności usługi.

 - Na koniec możesz spróbować wyczyścić pamięć podręczną klienta usługi Teams:

    1.  Całkowicie zamknij klienta stacjonarnego usługi Microsoft Teams. Kliknij prawym przyciskiem myszy **Teams** na pasku ikon i kliknij **Zamknij** albo otwórz Menedżer zadań i całkowicie zakończ proces.

    2.  Przejdź do Eksploratora plików i wpisz %appdata%\Microsoft\teams.

    3.  Po otwarciu katalogu będą widoczne następujące foldery:

         - W folderze **Application Cache** otwórz folder Cache i usuń wszystkie znajdujące się w nim pliki:  %appdata%\Microsoft\teams\application cache\cache.

        - W folderze **Blob_storage** usuń wszystkie pliki: %appdata%\Microsoft\teams\blob_storage.

        - W folderze **Cache**, usuń wszystkie pliki: %appdata%\Microsoft\teams\Cache.

        - W folderze **databases** usuń wszystkie pliki: %appdata%\Microsoft\teams\databases.

        - W folderze **GPUCache** usuń wszystkie pliki: %appdata%\Microsoft\teams\GPUcache.

        - W folderze **IndexedDB** usuń plik .db: %appdata%\Microsoft\teams\IndexedDB.

        - W folderze **Local Storage** usuń wszystkie pliki: %appdata%\Microsoft\teams\Local Storage.

        - Na koniec w folerze **tmp** usuń wszystkie pliki: %appdata%\Microsoft\teams\tmp.

    4. Ponownie otwórz klienta usługi Teams.

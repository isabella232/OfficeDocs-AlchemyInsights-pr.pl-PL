---
title: Problemy z logowaniem się do aplikacji Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695297"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Pusty ekran logowania w aplikacji Microsoft 365

Aby rozwiązać ten problem, spróbuj wykonać następujące czynności:
- Zainstaluj najnowsze aktualizacje dla [systemu Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [pakietu Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Resetowanie opcji programu Internet Explorer: Przejdź do **menu Narzędzia**  >  **Opcje internetowe**  >  **Advanced**  >  **Resetowanie ustawień programu Internet Explorer** (Zauważ, że ustawienia niestandardowe zostaną utracone), a następnie ponownie spróbuj zalogować się do pakietu Office.
- Wyłącz funkcję Windows Defender Application Guard (WDAG) lub jakąkolwiek podobną zaporę lub program antywirusowy:
    1. W panelu sterowania przejdź do pozycji **programy**, a następnie wybierz pozycję **Włącz lub wyłącz funkcje systemu Windows**.
    2. Jeśli funkcja Windows Defender Application Guard jest włączona, spróbuj ją wyłączyć.<br/>
    **Uwaga:** Być może będzie konieczne ponowne uruchomienie komputera.
- Upewnij się, że [wtyczka wam](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. BrokerPlugin AAD nie jest blokowana przez żadną aplikację lub zaporę bądź program antywirusowy.
- [Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0. (Np. \Software\Microsoft\Office\16.0\Common\Identity\)

Aby uzyskać więcej informacji, zobacz [problemy z połączeniem po zaktualizowaniu do pakietu Office 2016 kompilacja 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
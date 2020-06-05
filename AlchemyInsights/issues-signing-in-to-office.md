---
title: Problemy z logowaniem się do aplikacji usługi Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579911"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Pusty ekran logowania w aplikacjach usługi Microsoft 365

Aby rozwiązać ten problem, spróbuj wykonać następujące czynności:
- Zainstaluj najnowsze aktualizacje dla [systemu Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [pakietu Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Resetowanie opcji programu **Tools**Internet Explorer: Przejdź do  >  **opcji internetowych**  >  **Zaawansowane**  >  **resetowanie ustawień programu Internet Explorer** (zwróć uwagę, że utracisz ustawienia niestandardowe), a następnie spróbuj ponownie zalogować się do pakietu Office.
- Wyłącz ochronę aplikacji usługi Windows Defender (WDAG) lub podobną zaporę lub program antywirusowy:
    1. W Panelu sterowania przejdź do programu **Programy**, a następnie wybierz pozycję **Włącz lub wyłącz funkcje systemu Windows**.
    2. Jeśli usługa Windows Defender Application Guard jest włączona, spróbuj ją wyłączyć.<br/>
    **Uwaga:** Może być konieczne ponowne uruchomienie komputera.
- Upewnij się, że wtyczka Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie jest blokowana przez żadną aplikację lub zaporę/program antywirusowy.
- [Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16.0. (Np.: \Software\Microsoft\Office\16.0\Common\Identity\)

Aby uzyskać więcej informacji, zobacz [Problemy z połączeniem w logowanie po aktualizacji do pakietu Office 2016 kompilacji 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
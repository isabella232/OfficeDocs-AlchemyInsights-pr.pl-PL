---
title: Problemy z logowaniem się do aplikacji platformy Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833049"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Pusty ekran logowania w aplikacjach platformy Microsoft 365

Aby rozwiązać ten problem, wypróbuj następujące rozwiązania:
- Zainstaluj najnowsze aktualizacje dla systemu [Windows i](https://support.microsoft.com/help/4027667/windows-10-update) pakietu [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Zresetuj opcje programu Internet Explorer: Przejdź do narzędzia Opcje internetowe Zaawansowane Resetowanie ustawień programu Internet Explorer (pamiętaj, że utracisz ustawienia niestandardowe), a następnie ponownie spróbuj zalogować się  >    >    >   do pakietu Office.
- Wyłącz funkcję Windows Defender Application Guard (WDAG) lub podobną zaporę lub program antywirusowy:
    1. W Panelu sterowania przejdź do **opcji Programy**, a następnie wybierz pozycję Włącz lub wyłącz funkcje **systemu Windows.**
    2. Jeśli jest włączona funkcja Windows Defender Application Guard, spróbuj ją wyłączyć.<br/>
    **Uwaga:** Może być konieczne ponowne uruchomienie komputera.
- Upewnij się, że wtyczka Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie jest blokowana przez żadne aplikacje, zapory/programy antywirusowe.
- [Wyczyść poświadczenia pakietu Office za](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocą Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zmieniły się na 16.0. (Np.: \Software\Microsoft\Office\16.0\Common\Identity)\)

Aby uzyskać więcej informacji, zobacz Problemy z połączeniem podczas logowania po aktualizacji pakietu Office 2016 do kompilacji [16.0.7967 w systemie Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
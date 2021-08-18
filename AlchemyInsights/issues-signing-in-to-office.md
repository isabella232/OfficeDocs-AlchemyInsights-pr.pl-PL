---
title: Problemy z logowaniem się do Microsoft 365 aplikacji
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088046"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Pusty ekran logowania w Microsoft 365 aplikacji

Aby rozwiązać ten problem, wypróbuj następujące rozwiązania:
- Zainstaluj najnowsze aktualizacje dla aplikacji [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Zresetuj opcje programu Internet Explorer: Przejdź do narzędzia Opcje internetowe Zaawansowane Resetowanie ustawień programu  >    >    >  **Internet Explorer Ustawienia** (pamiętaj, że utracisz ustawienia niestandardowe), a następnie spróbuj zalogować się Office ponownie.
- Wyłącz Windows Defender Application Guard (WDAG) lub podobną zaporę bądź program antywirusowy:
    1. W Panelu sterowania przejdź do **opcji Programy**, a następnie wybierz pozycję Windows funkcje **programu .**
    2. Jeśli Windows Defender Application Guard jest włączona, spróbuj ją wyłączyć.<br/>
    **Uwaga:** Może być konieczne ponowne uruchomienie komputera.
- Upewnij się, że wtyczka Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie jest blokowana przez żadne aplikacje, zapory/programy antywirusowe.
- [Wyczyść Office przy użyciu](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menedżera poświadczeń Windows poświadczeń.<br/>
    **Uwaga:** Ścieżki rejestru w programie Office 2016 zmieniły się na 16.0. (Np.: \Software\Microsoft\Office\16.0\Common\Identity\)

Aby uzyskać więcej informacji, zobacz Problemy z połączeniem podczas logowania po aktualizacji do [kompilacji Office 2016 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)w Windows 10.
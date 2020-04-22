---
title: Problemy z logowaniem się do aplikacji pakietu Office
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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763011"
---
# <a name="issues-signing-in-to-office-apps"></a>Problemy z logowaniem się do aplikacji pakietu Office

Aby rozwiązać problemy z logowaniem w aplikacjach pakietu Office, spróbuj wykonać następujące czynności:

- Usuń wszystkie konta służbowe, z wyjątkiem konta, którego dotyczy problem, korzystając z ustawień systemu Windows > **access work or school**.
- [Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16.0. (Np.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otwórz aplikację pakietu Office, wybierz pozycję**Account** > **Wyloguj konto** **pliku** > . Następnie zaloguj się przy użyciu konta użytkownika z ważną licencją. Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jeśli używasz komputera Mac, zobacz temat [Nie mogę zalogować się do aplikacji pakietu Office 2016 dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Jeśli podczas nawiązywania błędów podczas łączenia się z programem Microsoft 365 przy użyciu pakietu Office 2013 wystąpią błędy, włącz nowoczesne uwierzytelnianie dla klienta pakietu Office.

Aby uzyskać więcej informacji, zobacz:
- [Nie można zalogować się do usługi Microsoft 365, azure lub intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Problemy z połączeniem podczas logowania po aktualizacji do kompilacji pakietu Office 2016 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Niestety, inne konto w organizacji jest już zalogowane na tym komputerze" w pakiecie Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Rozwiązywanie problemów z logowaniem z nowoczesnym uwierzytelnianiem pakietu Office podczas korzystania z usługi ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)
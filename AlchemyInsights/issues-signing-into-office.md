---
title: Problemy z zalogowaniem się do aplikacji pakietu Office
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
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938294"
---
# <a name="issues-signing-in-to-office-apps"></a>Problemy z zalogowaniem się do aplikacji pakietu Office

Aby rozwiązać problemy z logowaniem z aplikacji pakietu Office, wypróbuj następujące rozwiązania:

- Usuń wszystkie konta pracy, z wyjątkiem dotkniętych konta, przy użyciu ustawień systemu Windows > **dostępu do pracy i w szkole**.
- [Wyczyść Office poświadczeń](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otwórz aplikację pakietu Office, wybierz polecenie **plik** > **konta** > **Wyloguj się**. Następnie zaloguj się przy użyciu konta użytkownika z ważną licencją. Aby uzyskać szczegółowe informacje zobacz [konta w biurze](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Dla komputerów Macintosh Zobacz [nie można zalogować się do 2016 pakietu Office dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- W przypadku błędów podczas nawiązywania połączenia za pomocą pakietu Office 2013 Office 365, należy włączyć uwierzytelnianie nowoczesnych dla klienta pakietu Office.

Aby uzyskać więcej informacji, zobacz:
- [Nie możesz się zarejestrować usłudze Office 365, Azure lub Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Problemy z połączeniem w logowanie po aktualizacji do pakietu Office 2016 budować 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Niestety, innego konta z organizacji jest już zarejestrowany na tym komputerze" w pakiecie Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Logowanie Rozwiązywanie problemów związanych z uwierzytelnianiem nowoczesnych pakietu Office podczas korzystania z programu ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)
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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938293"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Ustalania komunikat "Niestety, innego konta z organizacji jest już zarejestrowany" aplikacje pakietu Office

Aby naprawić ten błąd, spróbuj wykonać następujące czynności:

- Usuń wszystkie konta pracy, z wyjątkiem dotkniętych konta, przy użyciu ustawień systemu Windows > **dostępu do pracy i w szkole**.
- [Wyczyść Office poświadczeń](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otwórz aplikację pakietu Office, wybierz polecenie **plik** > **konta** > **Wyloguj się**. Następnie zaloguj się przy użyciu konta użytkownika z ważną licencją. Aby uzyskać szczegółowe informacje zobacz [konta w biurze](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Dla komputerów Macintosh Zobacz [nie można zalogować się do 2016 pakietu Office dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Aby uzyskać więcej informacji, zobacz ["Niestety, innego konta z organizacji jest już zarejestrowany na tym komputerze" w pakiecie Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).
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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028050"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Naprawianie Microsoft 365 "Niestety, inne konto z Twojej organizacji jest już zalogowane"

Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:

- Usuń wszystkie konta służbowe, z wyjątkiem kont, których dotyczy problem, Windows Ustawienia > **uzyskaj dostęp do konta służbowego.**
- [Wyczyść Office przy użyciu](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menedżera poświadczeń Windows poświadczeń.<br/>
    **Uwaga:** Ścieżki rejestru w programie Office 2016 zmieniły się na 16.0. (Np.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otwórz konto aplikacja pakietu Office wybierz **pozycję Wyloguj**  >  **się z konta**  >  **pliku**. Następnie zaloguj się przy użyciu konta użytkownika z ważną licencją. Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jeśli używasz komputera Mac, zobacz temat [Nie mogę zalogować się do aplikacji pakietu Office 2016 dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Aby uzyskać więcej informacji, zobacz "Niestety, inne konto z Twojej organizacji jest już zalogowane na tym komputerze" w [programie Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
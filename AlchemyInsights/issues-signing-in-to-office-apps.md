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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833085"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Rozwiązywanie problemów z aplikacjami platformy Microsoft 365 "Niestety, inne konto z Twojej organizacji jest już zalogowane"

Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:

- Usuń wszystkie konta służbowe z wyjątkiem konta, którego dotyczy problem, za pomocą > systemu Windows **uzyskaj dostęp do konta służbowego.**
- [Wyczyść poświadczenia pakietu Office za](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocą Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zmieniły się na 16.0. (Np.: \Software\Microsoft\Office\16.0\Common\Identity)\)
- Otwórz aplikację pakietu Office, wybierz **pozycję Wyloguj**  >  **się z konta**  >  **pliku**. Następnie zaloguj się przy użyciu konta użytkownika z ważną licencją. Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jeśli używasz komputera Mac, zobacz temat [Nie mogę zalogować się do aplikacji pakietu Office 2016 dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Aby uzyskać więcej informacji, zobacz "Niestety, inne konto z Twojej organizacji jest już zalogowane [na tym komputerze" w psłudze Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
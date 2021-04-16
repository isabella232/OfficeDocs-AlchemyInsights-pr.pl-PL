---
title: Naprawianie aplikacji platformy Microsoft 365 Twoje konto jest w stanie błędu
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812546"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Naprawianie błędu "Twoje konto jest w złym stanie" w aplikacjach platformy Microsoft 365

Aby naprawić ten błąd, wypróbuj następujące opcje na komputerze, którego dotyczy problem:

- Otwórz aplikację pakietu Office i wybierz **pozycję Konto**  >  **pliku**  >  **Wyloguj się ze wszystkich kont.** Zaloguj się ponownie przy użyciu konta użytkownika z ważną licencją. Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Wyczyść poświadczenia pakietu Office za](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocą Menedżera poświadczeń systemu Windows.<br>
  **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zmieniły się na 16.0. Na przykład\Software\Microsoft\Office\16.0\Common\Identity\
- Jeśli podczas nawiązywania połączenia z usługą Office 365 za pomocą pakietu Office 2013 wystąpi błąd, włącz [nowoczesne uwierzytelnianie](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) dla klienta pakietu Office.

Aby uzyskać więcej informacji, zobacz Jak rozwiązywać problemy z aplikacjami nie przeglądarki, które nie mogą zalogować się do platformy [Microsoft 365, platformy Azure lub Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)


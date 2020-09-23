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
- "2574"
ms.openlocfilehash: a1e9844094dd164ca8bd5fb2a196161a5de0282f
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236135"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemy z logowaniem się do aplikacji Microsoft 365

Aby rozwiązać problemy z logowaniem się do aplikacji Microsoft 365, wypróbuj następujące opcje na komputerze, którego dotyczy problem:  

- W przypadku systemu Windows Zobacz [zalecenia dotyczące rozwiązywania typowych problemów z logowaniem](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Dla komputerów Mac zobacz  [nie można zalogować się do aplikacji Office 2016 dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Porada** Na urządzeniach z systemem Windows możemy zdiagnozować i automatycznie rozwiązać kilka typowych problemów z logowaniem do pakietu Office. Pobierz i uruchom  **[asystenta odzyskiwania i pomocy technicznej firmy Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** , aby korzystać z naszego narzędzia zautomatyzowanego.

**Uwaga:** Wyłączenie nowoczesnego uwierzytelniania (ADAL) lub zarządzania kontami sieci Web (WAM) w celu naprawienia problemów logowania lub aktywacji  **nie jest zalecane**. Jeśli podczas nawiązywania połączenia z programem Microsoft 365 przy użyciu pakietu Office 2013 występują błędy, upewnij się, że [włączono nowoczesne uwierzytelnianie](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  dla klienta pakietu Office.

Aby poznać konkretne akcje rozwiązywania problemów, zobacz:

[Problemy z połączeniem podczas logowania po aktualizacji do kompilacji pakietu Office 2016 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Nie można zalogować się do konta organizacji, takiego jak pakiet Office 365, Azure lub Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Jak rozwiązywać problemy z aplikacjami nieobsługującymi przeglądarki, które nie mogą zalogować się do pakietu Office 365, Azure lub Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Wielokrotne monity o poświadczenia w pakiecie Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)
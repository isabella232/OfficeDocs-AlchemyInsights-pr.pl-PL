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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744656"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemy z logowaniem do Aplikacje Microsoft 365

Uwaga: Jeśli korzystasz ze starszej wersji programu Windows (na przykład Windows 7 z dodatkiem SP1, Windows Server 2008 R2), użyj łatwej poprawki, aby włączyć domyślną wartość TLS 1.2. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Aby uzyskać więcej informacji, zobacz Aktualizowanie w celu włączenia [protokołów TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako domyślnych protokołów bezpiecznego w winieHTTP w programie Windows.

Aby rozwiązać problemy z logowaniem Microsoft 365, wypróbuj następujące opcje na komputerze, którego dotyczy problem:  

- Aby Windows, zobacz Rekomendacje na temat rozwiązywania typowych problemów [z logowaniem.](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- W przypadku komputerów Mac zobacz [Nie można zalogować się do Office 2016 dla komputerów Mac aplikacji](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Porada** Na komputerach z systemem Windows możemy diagnozować i automatycznie rozwiązywać wiele typowych problemów z logowaniem do pakietu Office. Pobierz i uruchom  **[Asystenta odzyskiwania i pomocy technicznej dla usługi Office 365](https://aka.ms/SaRA-OfficeSignInScenario)**, aby skorzystać z naszego zautomatyzowanego narzędzia.

**Uwaga:** Nie zaleca się wyłączania nowoczesnego uwierzytelniania (ADAL, Modern Authentication) ani zarządzania kontem sieci Web (WAM, Web Account Management) w celu rozwiązywania problemów z logowaniem lub **aktywacją.** Jeśli podczas nawiązywania połączenia z usługą Microsoft 365 w programie Office 2013 wystąpią błędy, włącz nowoczesne [uwierzytelnianie](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) dla Office klienta.

Aby uzyskać szczegółowe działania rozwiązywania problemów, zobacz:

[Problemy z połączeniem podczas logowania po aktualizacji do kompilacji pakietu Office 2016 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Nie możesz zalogować się do swojego konta organizacji, takiego jak Office 365, Azure lub Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Jak rozwiązywać problemy z aplikacjami nie przeglądarki, które nie mogą zalogować się do usługi Office 365, Azure lub Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Wielokrotnie był wyświetlany monit o poświadczenia w Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)
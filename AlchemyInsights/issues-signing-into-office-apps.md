---
title: Problemy z logowaniem się do aplikacji usługi Microsoft 365
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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579875"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Naprawianie komunikatu "Moduł Zaufana platforma komputera komputera nie działa prawidłowo"

Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:

- Zainstaluj najnowsze aktualizacje dla [systemu Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [pakietu Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16.0. (Np.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Wypróbuj [proces odzyskiwania użytkownika,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) aby naprawić błędy modułu TPM (Trusted Platform Module).
- Ustaw EnableADAL = 0, wykonując następujące kroki:  
    1. Kliknij prawym przyciskiem myszy przycisk Start systemu Windows, wybierz polecenie **Uruchom**, wpisz **regedit**, a następnie wybierz przycisk **OK**.
    2. Wybierz **pozycję Tak,** aby zezwolić Edytorowi rejestru na wprowadzanie zmian na urządzeniu.
    3. W Edytorze rejestru dodaj wartość DWORD **enableADAL** z ustawieniem **0** w obszarze HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Aby uzyskać więcej informacji, zobacz [Problemy z połączeniem w logowanie po aktualizacji do pakietu Office 2016 kompilacji 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
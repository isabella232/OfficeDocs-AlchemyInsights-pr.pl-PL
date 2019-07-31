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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938296"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Ustalania komunikat "moduł zaufanej platformy komputera nie działa poprawnie" aplikacje pakietu Office

Aby naprawić ten błąd, spróbuj wykonać następujące czynności:

- Zainstaluj najnowsze aktualizacje dla [systemu Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [pakietu Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Wyczyść Office poświadczeń](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Spróbuj [proces odzyskiwania użytkownika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) do naprawienia błędów moduł zaufanej platformy (TPM).
- Ustaw EnableADAL = 0, wykonując następujące czynności:  
    1. Kliknij prawym przyciskiem myszy przycisk Start systemu Windows, wybierz polecenie **Uruchom**, wpisz **polecenie regedit**, a następnie wybierz **OK**.
    2. Wybierz opcję **Tak,** aby umożliwić Edytora rejestru, aby wprowadzić zmiany do urządzenia.
    3. W Edytorze rejestru dodać wartość DWORD **EnableADAL** z ustawieniem **0** w obszarze HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Aby uzyskać więcej informacji zobacz [w logowanie po aktualizacji do pakietu Office 2016 build 16.0.7967 w systemie Windows 10 problemy z połączeniem](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
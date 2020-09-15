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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695189"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Rozwiązywanie problemów z aplikacjami Microsoft 365 "moduł zaufanej platformy na komputerze nie działa prawidłowo"

Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:

- Zainstaluj najnowsze aktualizacje dla [systemu Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [pakietu Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0. (Np. \Software\Microsoft\Office\16.0\Common\Identity\)
- Spróbuj naprawić błędy modułu TPM (Trusted Platform Module) za pomocą [procesu odzyskiwania](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) .
- Ustaw EnableADAL = 0, wykonując następujące czynności:  
    1. Kliknij prawym przyciskiem myszy przycisk Start systemu Windows, wybierz pozycję **Uruchom**, wpisz ciąg **regedit**, a następnie wybierz przycisk **OK**.
    2. Wybierz pozycję **tak** , aby zezwolić edytorowi rejestru na wprowadzanie zmian na urządzeniu.
    3. W Edytorze rejestru Dodaj wartość DWORD **EnableADAL** z ustawieniem **0** w obszarze HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Aby uzyskać więcej informacji, zobacz [problemy z połączeniem po zaktualizowaniu do pakietu Office 2016 kompilacja 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
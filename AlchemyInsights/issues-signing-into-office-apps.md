---
title: Problemy z logowaniem się do aplikacji platformy Microsoft 365
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
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709116"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Naprawianie komunikatu "Moduł Zaufana platforma komputera nie działa poprawnie" w aplikacjach platformy Microsoft 365

Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:

- Zainstaluj najnowsze aktualizacje dla systemu [Windows i](https://support.microsoft.com/help/4027667/windows-10-update) pakietu [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Wyczyść poświadczenia pakietu Office przy](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) użyciu Menedżera poświadczeń systemu Windows.<br/>
    **Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zmieniły się na 16.0. (Np.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Wypróbuj proces [odzyskiwania użytkowników, aby](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) naprawić błędy modułu TRUSTED Platform Module (TPM).
- Ustaw wartość EnableADAL = 0, korzystając z następujących kroków:  
    1. Kliknij prawym przyciskiem myszy przycisk Start systemu Windows, wybierz polecenie **Uruchom,** wpisz **polecenie regedit,** a następnie wybierz przycisk **OK.**
    2. Wybierz **pozycję Tak,** aby zezwolić Edytorowi rejestru na wprowadzanie zmian na urządzeniu.
    3. W Edytorze rejestru dodaj wartość DWORD wartości **EnableADAL** z ustawieniem **0** w obszarze HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Aby uzyskać więcej informacji, zobacz Problemy z połączeniem podczas logowania się po aktualizacji do pakietu [Office 2016 kompilacja 16.0.7967 w systemie Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
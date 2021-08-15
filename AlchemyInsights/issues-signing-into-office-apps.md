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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986901"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Naprawianie Microsoft 365 "Moduł zaufanej platformy komputera nie działa poprawnie"

Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:

- Zainstaluj najnowsze aktualizacje dla aplikacji [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Wyczyść Office przy użyciu](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) menedżera poświadczeń Windows poświadczeń.<br/>
    **Uwaga:** Ścieżki rejestru w programie Office 2016 zmieniły się na 16.0. (Np.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Spróbuj wykonać [proces odzyskiwania użytkowników,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) aby naprawić błędy modułu TPM.
- Ustaw wartość EnableADAL = 0, korzystając z następujących kroków:  
    1. Kliknij prawym przyciskiem myszy Windows Start, wybierz **pozycję Uruchom,** **wpisz regedit**, a następnie wybierz przycisk **OK.**
    2. Wybierz **pozycję Tak,** aby zezwolić Edytorowi rejestru na zmiany wprowadzone na urządzeniu.
    3. W Edytorze rejestru dodaj wartość DWORD wartości **EnableADAL** z ustawieniem **0** w obszarze HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Aby uzyskać więcej informacji, zobacz Problemy z połączeniem podczas logowania po aktualizacji do [kompilacji Office 2016 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)w Windows 10.
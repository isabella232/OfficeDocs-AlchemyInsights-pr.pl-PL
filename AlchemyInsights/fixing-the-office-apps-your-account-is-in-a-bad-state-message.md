---
title: Naprawianie aplikacji pakietu Office Twoje konto jest w złym stanie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969671"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Naprawianie błędu aplikacji pakietu Office "Twoje konto jest w złym stanie"

Aby naprawić ten błąd, wypróbuj następujące opcje na komputerze, którego dotyczy problem:

- Otwórz aplikację pakietu Office, wybierz pozycję**Wyloguj****konto** >  **pliku** > wszystkich kont . Zaloguj się ponownie przy użyciu konta użytkownika z ważną licencją. Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.<br>
  **Uwaga:** Ścieżki rejestru pakietu Office 2016 zostały zmienione na 16.0. Na przykład \Software\Microsoft\Office\16.0\Common\Identity\
- Na komputerze, którego dotyczy problem, ustaw enableadal = 0, wykonując następujące kroki:  
     1. Kliknij prawym przyciskiem myszy przycisk Windows i wybierz polecenie **Uruchom**. W polu **Otwórz** wpisz **regedit,** a następnie wybierz **przycisk OK**.
     2. Po wyświetleniu monitu wybierz **pozycję Tak,** aby zezwolić Edytorowi rejestru na wprowadzanie zmian na urządzeniu.
    3. W Edytorze rejestru dodaj wartość DWORD EnableADAL z ustawieniem 0 w obszarze HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.
- Jeśli podczas łączenia się z usługi Office 365 przy użyciu pakietu Office 2013 wystąpi błąd, [włącz nowoczesne uwierzytelnianie](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) dla klienta pakietu Office.

Aby uzyskać więcej informacji, zobacz [Jak rozwiązywać problemy z aplikacjami nieprzeglądarkowymi, które nie mogą zalogować się do usługi Office 365, platformy Azure lub usługi Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)


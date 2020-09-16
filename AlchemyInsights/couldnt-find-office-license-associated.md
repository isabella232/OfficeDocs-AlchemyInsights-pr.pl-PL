---
title: Rozwiązywanie problemów z aplikacjami Microsoft 365 nie można znaleźć wiadomości skojarzonych z licencjami pakietu Office
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747705"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Rozwiązywanie problemów z aplikacjami Microsoft 365 "nie można znaleźć wiadomości skojarzonych z licencjami pakietu Office"

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i ustawień serwera proxy, aby upewnić się, że nie blokuje dostępu do Internetu aplikacjom Microsoft 365. Zobacz [adresy URL i zakresy adresów IP w programie Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Usuń i [ponownie Przypisz licencję pakietu Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) dla użytkownika, którego dotyczy problem. 
3. Otwórz aplikację pakietu Office i [Wyloguj się](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z istniejących kont użytkowników.
4. Przejdź do obszaru Ustawienia systemu **Windows > konta**  >  **e-mail & konta**, a następnie usuń wszystkie konta służbowe oprócz konta, którego dotyczy problem.
5. Przejdź do obszaru Ustawienia systemu Windows > **konto**  >  **służbowe lub szkolne**, a następnie odłącz wszystkie konta służbowe oprócz konta, którego dotyczy problem.
6. Zresetuj stan aktywacji pakietu Office. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Zaloguj się](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) przy użyciu konta użytkownika, którego dotyczy problem.

Aby uzyskać dodatkowe rozwiązania dotyczące rozwiązywania problemów, zobacz [nielicencjonowany produkt i błędy aktywacji w pakiecie Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).
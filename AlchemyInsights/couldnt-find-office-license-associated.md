---
title: Naprawianie aplikacji pakietu Office Nie można znaleźć wiadomości skojarzonej z licencjami pakietu Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 887be4bee2bd1562bdc3b29783e9deafe47d8d57
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505877"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>Rozwiązywanie komunikatów "Nie można znaleźć skojarzonych licencji pakietu Office"

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują dostępu do Internetu w aplikacjach pakietu Office. Zobacz [adresy URL i zakresy adresów IP usługi Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Usuń i [ponownie przypisz licencję pakietu Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) dla użytkownika, którego dotyczy problem. 
3. Otwórz aplikację pakietu Office i [wyloguj się](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z istniejących kont użytkowników.
4. Przejdź do pozycji Ustawienia **Accounts**systemu Windows >  >  **kontach e-mail & konta i**usuń wszystkie konta służbowe z wyjątkiem konta, którego dotyczy problem.
5. Przejdź do pozycji Ustawienia **Accounts**systemu Windows >  >  **Dostęp do kont w szkole**i odłącz wszystkie konta służbowe z wyjątkiem konta, którego dotyczy problem.
6. Zresetuj stan aktywacji pakietu Office. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Zaloguj się](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) przy użyciu konta użytkownika, którego dotyczy problem.

Aby uzyskać dodatkowe rozwiązania do rozwiązywania problemów, zobacz [Nielicencjonowany produkt i błędy aktywacji w pakiecie Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).
---
title: Naprawianie aplikacji pakietu Office nie można odnaleźć wiadomości związanych z licencjami pakietu Office
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
ms.openlocfilehash: 1820cdb83a1adf36b4e7d0898ecdf8097eb6f0f3
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627928"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>Naprawianie wiadomości aplikacji pakietu Office "nie można odnaleźć skojarzonych licencji pakietu Office"

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory sieciowej, oprogramowania antywirusowego i serwera proxy, aby potwierdzić, że nie blokują dostępu do Internetu aplikacjom pakietu Office. Zobacz [adresy url 365 pakietu Office i zakresy adresów IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Usuń i [ponownie Przypisz licencję pakietu Office](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) dla użytkownika, którego dotyczy luka. 
3. Otwórz aplikację pakietu Office i [Wyloguj](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) się z istniejących kont użytkowników.
4. Przejdź do ustawienia systemu Windows **>** > konta**e-mail & konta**i Usuń wszystkie konta pracy z wyjątkiem konta, którego dotyczy luka.
5. Przejdź do ustawienia systemu Windows > **konta** > **dostępu do pracy lub szkoły**, a następnie odłącz wszystkie konta pracy z wyjątkiem konta, którego dotyczy problem.
6. Zresetuj stan aktywacji pakietu Office. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Zaloguj się](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) przy użyciu konta użytkownika, którego dotyczy luka.

Aby uzyskać dodatkowe rozwiązania dotyczące rozwiązywania problemów, zobacz [nielicencjonowany produkt i błędy aktywacji w pakiecie Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).
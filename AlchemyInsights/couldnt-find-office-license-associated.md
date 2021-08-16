---
title: Rozwiązywanie Microsoft 365 wiadomości z skojarzoną licencją pakietu Office
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
- "3421"
- "9001426"
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069614"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Naprawianie Microsoft 365 "Nie można znaleźć skojarzonych licencji pakietu Office"

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu do Internetu Microsoft 365 aplikacji. Zobacz [Microsoft 365 URL i zakresów adresów IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Usuń i [ponownie przypisz licencję Office użytkownika,](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) którego dotyczy problem. 
3. Otwórz aplikacja pakietu Office i [wyloguj się](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z istniejących kont użytkowników.
4. Przejdź do Windows Ustawienia > **Konta**  >  **e& e-mail** i usuń wszystkie konta służbowe z wyjątkiem konta, którego dotyczy problem.
5. Przejdź do Windows Ustawienia > **Konta Uzyskaj** dostęp do konta służbowego i odłącz wszystkie konta służbowe z wyjątkiem konta, którego dotyczy  >  problem.
6. Zresetuj stan aktywacji pakietu Office. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Zaloguj się przy](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) użyciu konta użytkownika, którego dotyczy problem.

Aby uzyskać dodatkowe rozwiązania problemów, zobacz Błędy "Produkt bez licencji" i [błędy](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)aktywacji w Office.
---
title: Rozwiązywanie problemów z aplikacjami platformy Microsoft 365 Nie można odnaleźć skojarzonego komunikatu z licencjami pakietu Office
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
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816498"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Naprawianie komunikatu "Nie można znaleźć skojarzonych licencji pakietu Office" dla aplikacji platformy Microsoft 365

Jeśli zostanie wyświetlony ten komunikat, spróbuj wykonać następujące czynności:

1. Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu do Internetu do aplikacji platformy Microsoft 365. Zobacz Adresy URL i zakresy adresów [IP platformy Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Usuń i [ponownie przyzmij licencję pakietu Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) dla użytkownika, którego dotyczy problem. 
3. Otwórz aplikację pakietu Office i [wyloguj się](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z istniejących kont użytkowników.
4. Przejdź do pozycji Ustawienia systemu Windows > **Konta**  >  **e-& konta e-mail** i usuń wszystkie konta służbowe z wyjątkiem kont, których dotyczy problem.
5. Przejdź do pozycji Ustawienia systemu Windows > **Konta** Uzyskaj dostęp do konta służbowego i odłącz wszystkie konta służbowe z wyjątkiem konta, którego  >  dotyczy problem.
6. Zresetuj stan aktywacji pakietu Office. [Dowiedz się, jak to zrobić](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Zaloguj się przy](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) użyciu konta użytkownika, którego dotyczy problem.

Aby uzyskać dodatkowe rozwiązania problemów, zobacz [Błędy "Produkt bez licencji" i błędy aktywacji w psłudze Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
---
title: Ustawianie automatycznych odpowiedzi dla skrzynki pocztowej
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046618"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Ustawianie automatycznych odpowiedzi dla skrzynki pocztowej użytkownika

**Metoda 1**

1. Zaloguj się do portalu platformy Microsoft 365.

2. Przejdź do pozycji **Użytkownicy > Aktywni użytkownicy** (lub **Grupy > Udostępnione skrzynki pocztowe** w przypadku konfigurowania ustawień dla udostępnionej skrzynki).

3. Wybierz użytkownika, który ma skrzynkę pocztową programu Microsoft Exchange.

4. W menu wysuwanym po prawej stronie przejdź do pozycji **Ustawienia poczty > Odpowiedzi automatyczne** (w przypadku udostępnionej skrzynki pocztowej wystarczy kliknąć pozycję **Odpowiedzi automatyczne** w menu wysuwanym).

**Metoda 2**

1. Zaloguj się do portalu administracyjnego platformy Microsoft 365 przy użyciu poświadczeń administratora usługi.

2. Rozwiń pozycję **Centra administracyjne**, a następnie kliknij pozycję **Exchange**.

3. Kliknij obraz w prawym górnym rogu, kliknij pozycję **Inny użytkownik**, a następnie wybierz skrzynkę pocztową użytkownika, którą chcesz zmienić.

4. Po lewej stronie wybierz pozycję **Opcje**, kliknij pozycję **Organizuj wiadomości e-mail**, a następnie kliknij pozycję **Odpowiedzi automatyczne.**

**Metoda 3**

Uruchom następujące polecenie cmdlet w module programu PowerShell dla usługi Exchange Online:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Aby uzyskać więcej informacji o tym poleceniu cmdlet, zobacz [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).

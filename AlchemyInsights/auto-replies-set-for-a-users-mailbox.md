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
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820944"
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

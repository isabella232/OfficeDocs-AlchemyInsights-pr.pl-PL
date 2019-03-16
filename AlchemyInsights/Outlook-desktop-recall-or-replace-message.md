---
title: Odwołanie w programie Outlook pulpitu lub zamienianie wiadomości e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657053"
---
# <a name="recall-or-replace-an-email-message"></a>Odwoływanie lub zamienianie wiadomości e-mail

- Jako administrator możesz **odwoływania wiadomości w imieniu użytkowników przy użyciu programu PowerShell**. Nie można odwołać wiadomości z Centrum administracyjnego.
- Możesz **tylko odwoływania wiadomości, które są wysyłane do osoby w organizacji**. Jeśli wiadomość została wysłana na adres Gmail, na przykład, nie można wywołać ją.
- Możesz **tylko odwoływania wiadomości wysłane z Outlook 2016 na komputerze PC**. Jeśli użytkownik wysyła wiadomości za pomocą programu Outlook w sieci web lub programu Outlook dla komputerów Macintosh, nie może je wycofać.

Aby odwołać lub zastąpić wiadomość e-mail:

1. W okienku folderów po lewej stronie okna programu Outlook zaznacz folder Elementy wysłane.
1. Kliknij dwukrotnie wiadomość, którą chcesz odwołać go otworzyć.
1. Wybierz kartę **wiadomość** , a następnie wybierz **Akcje** > **Odwołaj tę wiadomość**.
1. Wybierz **usunąć nieprzeczytane kopie tej wiadomości** lub **usunąć nieprzeczytane kopie i zastąpić je nową wiadomością**, a następnie wybierz przycisk **OK**.
1. Jeśli wysyłasz wiadomość wymiany redagowania wiadomości, a następnie zaznacz pole wyboru **Wyślij**.
1. Powodzenie lub niepowodzenie odwołania wiadomości zależy od ustawień odbiorcy w programie Outlook. Aby sprawdzić na przypomnienie, w [tym](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)artykule czynności.

Wyszukiwanie i usuwanie wiadomości e-mail w organizacji

- Jeśli nie jesteś administratorem globalnym, Twoje konto musi dodane do roli Menedżer zbierania elektronicznych materiałów dowodowych lub Rola zarządzania zgodności wyszukiwania do wyszukiwania wiadomości. Aby usunąć wiadomości, będziesz musiał przyłączyć się do grupy ról Zarządzanie organizacją lub Rola zarządzania wyszukiwania i czyszczenie. W [Centrum zabezpieczeń i zgodności](https://go.microsoft.com/fwlink/?linkid=2083731)są przypisane uprawnienia dla tych ról.
- [Tworzenie zawartości wyszukiwania](https://docs.microsoft.com/office365/securitycompliance/content-search) , aby odnaleźć wiadomości do usunięcia.
- [Podłącz do bezpieczeństwa i środowiska PowerShell Centrum zgodności](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jeśli używasz wieloczynnikowe uwierzytelnianie Zobacz [Łączenie z zabezpieczeń usługi Office 365 oraz środowiska PowerShell Centrum zgodności za pomocą wieloczynnikowe uwierzytelnianie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).
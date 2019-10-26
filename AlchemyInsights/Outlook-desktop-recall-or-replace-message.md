---
title: Outlook Desktop przywoływanie lub zastępowanie wiadomości e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496121"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Odwoływanie lub zastępowanie wiadomości e-mail programu Outlook

- Jako administrator można **przywołać wiadomości w imieniu użytkowników przy użyciu programu PowerShell**. Nie można przywoływać wiadomości z centrum administracyjnego.
- Można **przywoływać tylko te wiadomości, które są wysyłane do osób w organizacji**. Jeśli wiadomość została wysłana na adres Gmail, na przykład nie możesz jej przypomnieć.
- **Wiadomości wysłane z programu Outlook 2016 można przywoływać tylko na komputerze**. Jeśli użytkownik wyśle wiadomość za pomocą programu Outlook dla komputerów Macintosh lub Outlook w sieci Web, nie można go przypomnieć.

Aby przywołać lub zamienić wiadomość e-mail:

1. W okienku folderów po lewej stronie okna programu Outlook wybierz folder Elementy wysłane.
1. Kliknij dwukrotnie wiadomość, którą chcesz przypomnieć, aby ją otworzyć.
1. Wybierz kartę **wiadomość** , a następnie wybierz **Akcje** > **Przywołaj tę wiadomość**.
1. Wybierz opcję **Usuń nieprzeczytane kopie tej wiadomości** lub **Usuń nieprzeczytane kopie i Zastąp ją nową wiadomością**, a następnie wybierz **przycisk OK**.
1. Jeśli wysyłasz wiadomość zastępczą, Skomponuj wiadomość, a następnie wybierz **Wyślij**.
1. Powodzenie lub niepowodzenie odwołania wiadomości zależy od ustawień adresata w programie Outlook. Aby uzyskać instrukcje dotyczące sprawdzania wycofywania, zobacz [ten artykuł](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Wyszukiwanie i usuwanie wiadomości e-mail w organizacji

- Jeśli nie jesteś administratorem globalnym, Twoje konto musi zostać dodane do roli menedżera zbierania elektronicznych materiałów dowodowych lub roli zarządzania wyszukiwania zgodności w celu wyszukania wiadomości. Aby usunąć wiadomości, należy przyłączyć się do grupy ról Zarządzanie organizacją lub wyszukiwanie i czyszczenie roli zarządzania. Uprawnienia dla tych ról są przypisywane w [Centrum zabezpieczeń i zgodności](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Utwórz Wyszukiwanie zawartości](https://docs.microsoft.com/office365/securitycompliance/content-search) , aby znaleźć wiadomość do usunięcia.
- [Połącz się z zabezpieczeniami i centrum zgodności środowiska PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jeśli korzystasz z uwierzytelniania wieloskładnikowego, zobacz [nawiązywanie połączenia z pakietem Office 365 Security i centrum zgodności środowiska PowerShell przy użyciu uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).
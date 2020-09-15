---
title: Program Outlook Desktop odwoływanie lub zamienianie wiadomości e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664000"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Odwoływanie lub zamienianie wiadomości e-mail programu Outlook

- Jako administrator możesz **odwołać wiadomości w imieniu użytkowników przy użyciu programu PowerShell**. Nie można odwołać wiadomości z centrum administracyjnego.
- Możesz **odwołać tylko wiadomości wysłane do osób w organizacji**. Jeśli wiadomość została wysłana na adres Gmail, na przykład nie można jej odwołać.
- **Wiadomości wysłane z programu Outlook 2016 można odwołać tylko na komputerze PC**. Jeśli użytkownik wyśle wiadomość za pomocą programu Outlook dla komputerów Mac lub aplikacji Outlook w sieci Web, nie można jej odwołać.

Aby odwołać lub zamienić wiadomość e-mail:

1. W okienku folderów po lewej stronie okna programu Outlook wybierz folder Elementy wysłane.
1. Kliknij dwukrotnie wiadomość, którą chcesz odwołać, aby ją otworzyć.
1. Wybierz kartę **wiadomość** , a następnie wybierz pozycję **Akcje**  >  **odwołaj tę wiadomość**.
1. Wybierz pozycję **Usuń nieprzeczytane kopie tej wiadomości** lub **Usuń nieprzeczytane kopie i zastąp je nową wiadomością**, a następnie wybierz przycisk **OK**.
1. Jeśli wysyłasz wiadomość zastępującą, Zredaguj wiadomość, a następnie wybierz pozycję **Wyślij**.
1. Sukces lub niepowodzenie odwołania wiadomości zależy od ustawień adresata w programie Outlook. Procedurę sprawdzania odwołania można znaleźć w [artykule](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Wyszukiwanie i usuwanie wiadomości e-mail w organizacji

- Jeśli nie jesteś administratorem globalnym, konto musi zostać dodane do roli menedżera zbierania elektronicznych materiałów dowodowych lub roli zarządzania wyszukiwaniem zgodności w celu wyszukania wiadomości. Aby usunąć wiadomości, musisz przyłączyć się do grupy ról zarządzania organizacją lub wyszukiwania i usuwania. Uprawnienia do tych ról są przypisywane w [Centrum zabezpieczeń i zgodności](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Utwórz Wyszukiwanie zawartości](https://docs.microsoft.com/microsoft-365/compliance/content-search) , aby znaleźć wiadomość, którą chcesz usunąć.
- [Nawiązywanie połączenia z programem PowerShell w centrum zabezpieczeń i zgodności](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jeśli korzystasz z uwierzytelniania wieloskładnikowego, zobacz [nawiązywanie połączenia z programem Microsoft 365 Security and zgodna Center za pomocą uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).
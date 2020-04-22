---
title: Odwoływanie lub zastępowanie wiadomości e-mail w programie Outlook Desktop
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687520"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Odwoływanie lub zastępowanie wiadomości e-mail programu Outlook

- Jako administrator możesz **odwoływać wiadomości w imieniu użytkowników korzystających z programu PowerShell**. Nie można odwołać wiadomości z centrum administracyjnego.
- Można **odwoływać tylko wiadomości, które są wysyłane do osób w organizacji**. Jeśli na przykład wiadomość została wysłana na adres Gmaila, nie możesz jej odwołać.
- Można **odwoływać tylko wiadomości wysyłane z programu Outlook 2016 na komputerze**. Jeśli użytkownik wysyła wiadomość za pomocą programu Outlook dla komputerów Mac lub programu Outlook w sieci Web, nie można jej odwołać.

Aby odwołać lub zastąpić wiadomość e-mail:

1. W okienku folderów po lewej stronie okna programu Outlook wybierz folder Elementy wysłane.
1. Kliknij dwukrotnie wiadomość, którą chcesz przywołać, aby ją otworzyć.
1. Wybierz kartę **Wiadomość,** a następnie wybierz pozycję **Akcje** > **Przywołuje tę wiadomość**.
1. Wybierz **pozycję Usuń nieprzeczytane kopie tej wiadomości** lub Usuń **nieprzeczytane kopie i zastąp nową wiadomością**, a następnie wybierz przycisk **OK**.
1. Jeśli wysyłasz wiadomość zastępczą, skomponuj ją, a następnie wybierz pozycję **Wyślij**.
1. Powodzenie lub niepowodzenie odwołania wiadomości zależy od ustawień adresata w programie Outlook. Aby uzyskać kroki, aby sprawdzić na wycofanie, zobacz [ten artykuł](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Wyszukiwanie i usuwanie wiadomości e-mail w organizacji

- Jeśli nie jesteś administratorem globalnym, twoje konto musi zostać dodane do roli Menedżera zbierania elektronicznych materiałów dowodowych lub roli zarządzania wyszukiwaniem zgodności, aby wyszukiwać wiadomości. Aby usunąć wiadomości, musisz dołączyć do grupy ról Zarządzanie organizacją lub roli zarządzania wyszukiwaniem i przeczyszczaniem. Uprawnienia dla tych ról są przypisywane w [Centrum zabezpieczeń i zgodności](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Utwórz wyszukiwanie zawartości,](https://docs.microsoft.com/office365/securitycompliance/content-search) aby znaleźć wiadomość do usunięcia.
- [Połącz się z centrum zabezpieczeń i zgodności programu PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jeśli używasz uwierzytelniania wieloskładnikowego, zobacz [Łączenie się z programem Microsoft 365 security and Compliance Center PowerShell przy użyciu uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).